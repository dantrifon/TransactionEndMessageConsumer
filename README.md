# TransactionEndMessageConsumer
This is a .NET console application that listens to a RabbitMQ queue and extracts the "TransactionBarcode" field from incoming messages. It uses the RabbitMQ.Client library to connect to the queue and Newtonsoft.Json to deserialize the messages.
