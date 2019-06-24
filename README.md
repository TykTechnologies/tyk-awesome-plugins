# tyk-awesome-plugins

## Security
- [Bot detection](https://github.com/TykTechnologies/tyk-plugin-bot-detection): block clients based on the user agent string.

## Logging

- [Loggly](https://github.com/TykTechnologies/tyk-plugin-loggly): log request metrics to [Loggly](https://www.loggly.com/).

## Others/Extensions
- [Queue](https://github.com/TykTechnologies/tyk-plugin-queue): send items to a queue server (see the repository for additional information).
- [Webhook](https://github.com/TykTechnologies/tyk-plugin-webhook): trigger a webhook.
- [Correlation](https://github.com/TykTechnologies/tyk-plugin-correlation): identify and trace your requests.

## Plugin demos

## .NET / C# #

This demo covers a basic Pre hook and an authentication middleware, based on Microsoft SQL Server, code & docs available [here](https://github.com/TykTechnologies/tyk-plugin-demo-dotnet).

## Python

This demo performs header injection using Pre/Post hooks. Code available [here](https://github.com/TykTechnologies/tyk-plugin-demo-python).

## Ruby

This demo performs header injection using a Pre hook. Code available [here](https://github.com/TykTechnologies/tyk-plugin-demo-ruby).

## Lua

This demo performs header injection using a Pre hook. Code available [here](https://github.com/TykTechnologies/tyk-plugin-demo-lua).

## Java

This demo performs custom authentication using a gRPC server with Java Logic.  It also takes advantage of Tyk's ID extraction caching mechanism.
https://github.com/sedkis/tyk-plugin-custom-auth-java

## Javascript / JSVM

This demo plugin performs [dynamic header transformation](https://gist.github.com/asoorm/4dd9f4361ad92d2f7201141fc09cbcb1) using a Pre Hook.

## GoLang / RabbitMQ / RPC

This demo validates an incoming `POST` request and upon success, publishes the message onto RabbitMQ queue. A worker picks up the request, creates a response and replies to a temporary `reply_to` queue with appropriate `correlation_id`. [Tyk GoLang RabbitMQ gRPC Middleware](https://github.com/asoorm/tyk-rmq-middleware).

## GoLang / AWS Lambda

This demo allows you to specify your hook name as your lambda function name. The gRPC plugin then invokes it and responds.

https://github.com/TykTechnologies/tyk-mw-grpcgo-lambda

## GoLang - Native GO Plugin Authentication via AWS DynamoDB

https://github.com/TykTechnologies/native-go-auth-middleware

Built to be run natively as a package by Tyk Gateway, will check basic auth credentials against AWS' DynamoDB

## Protocol Buffer definitions / bindings

You may find the latest Protocol Buffer definitions in [this repository](https://github.com/TykTechnologies/tyk-protobuf).
