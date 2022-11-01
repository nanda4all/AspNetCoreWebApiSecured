# AspNetCoreWebApiSecured

Secure ASP.NET Core Web API using API Key Authentication and Using a Custom Middleware

1) Using a ApiKey

Implementing the IAsyncActionFilter Interface will be able to intercept the call request, process it and then route the request back to the controller
[AttributeUsage(validOn: AttributeTargets.Class | AttributeTargets.Method)] -> This means, the attribute can be used in Class as well as Method

2) Using a Custom Middleware
With a custom ASP.NET Core Middleware you are able to intercept and process the request object in a single place.

You can intercept each and every request that comes to your published web APIs and tap into the request headers collection and search for the API key header and validate its value.
