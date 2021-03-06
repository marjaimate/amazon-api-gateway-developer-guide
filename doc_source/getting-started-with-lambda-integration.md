# Build an API Gateway API with Lambda Integration<a name="getting-started-with-lambda-integration"></a>

 To build an API with Lambda integrations, you can use Lambda proxy integration or Lambda custom integration\. 

In Lambda proxy integration, the input to the integrated Lambda function can be expressed as any combination of request headers, path variables, query string parameters, and body\. In addition, the Lambda function can use API configuration settings to influence its execution logic\. For an API developer, setting up a Lambda proxy integration is simple\. Other than choosing a particular Lambda function in a given region, you have little else to do\. API Gateway configures the integration request and integration response for you\. Once set up, the integrated API method can evolve with the backend without modifying the existing settings\. This is possible because the backend Lambda function developer parses the incoming request data and responds with desired results to the client when nothing goes wrong or responds with error messages when anything goes wrong\.

In Lambda custom integration, you must ensure that input to the Lambda function is supplied as the integration request payload\. This implies that you, as an API developer, must map any input data the client supplied as request parameters into the proper integration request body\. You may also need to translate the client\-supplied request body into a format recognized by the Lambda function\. 

**Topics**
+ [Build an API Gateway API with Lambda Proxy Integration](api-gateway-create-api-as-simple-proxy-for-lambda.md)
+ [Build an API Gateway API with Cross\-Account Lambda Proxy Integration](apigateway-cross-account-lambda-integrations.md)
+ [Build an API Gateway API with Custom Lambda Integration](getting-started-lambda-non-proxy-integration.md)