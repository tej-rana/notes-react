# Notes React in AWS
Basic Notes App in React that is backed by aws cdk (nodejs) to setup Infrastructure. The backend is serverless consisting of Lambda behind API Gateway.
All the infrastructure is created with SST (serverless stack) which uses aws cdk. They currently do not support C# but this will come out soon.

## Why use SST?
It makes live development possible with web sockets listening for changes to push to remote dev stack. It also helps to organise stacks (api gateway, s3 bucket,
cognito user pool) and actual processing logic (lamda).

## Pre-requisites

You will need aws-cli, signed in with an aws account (this is where the code gets published) and latest version of node installed.

## Running
Run `npm i` to install all the packages
Run `npx sst start` to deploy the stacks
(Note you will need to modify the region to your account's region. This is in sst.json)

## Testing
Look inside `curl.txt`. You will need to update the parameters to make curl requests. 

Running unit tests is straightforward. 
Enter `npx sst test`




