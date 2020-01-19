# DynamoDB   

[AWS Tutorial on Dynamo](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/GettingStarted.Python.html)

## Install a local DynomoDB Server

[Download Here](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html)


`java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb`


You can start writing applications. To access DynamoDB running locally, use the --endpoint-url parameter. For example, use the following command to list DynamoDB tables.

`aws dynamodb list-tables --endpoint-url http://localhost:8000`
