# DynamoDB   

[AWS Tutorial on Dynamo](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/GettingStarted.Python.html)

## Install a local DynomoDB Server

[Download Here](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html)


Use the following command to start the local server:  
`java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb`


Use the following command to list DynamoDB tables.

`aws dynamodb list-tables --endpoint-url http://localhost:8000`  

## Modifying the Code to Use the DynamoDB Service
To use the DynamoDB web service, you must change the endpoint in your application. To do this, modify the following line:

`dynamodb = boto3.resource('dynamodb',endpoint_url="http://localhost:8000")`

For example, if you want to use the `us-west-2` Region, change the code to the following.

`dynamodb = boto3.resource('dynamodb',region_name='us-west-2')`
