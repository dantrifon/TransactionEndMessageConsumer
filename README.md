Transaction End Message Consumer

This is a .NET console application that listens to a RabbitMQ queue and extracts the "TransactionBarcode" field from incoming messages. It uses the RabbitMQ.Client library to connect to the queue and Newtonsoft.Json to deserialize the messages.

The app prompts the user to enter a queue name or retrieves it from the app.config file, then declares the queue and begins listening for messages. When a message is received, it attempts to extract the TransactionBarcode field. If the field is found, it prints its value to the console along with the date and time of consumption. If the field is not found, it prints an error message to the console.

The app requires a running instance of RabbitMQ and a queue to listen to. You can configure the queue name in the app.config file or enter it at runtime when prompted.
Dependencies

    .NET Framework 4.7.2
    RabbitMQ.Client 6.2.2
    Newtonsoft.Json 13.0.1
