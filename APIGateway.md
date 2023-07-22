Amazon API Gateway is an AWS service for creating, publishing, maintaining, monitoring, and securing REST, HTTP, and WebSocket APIs at any scale
### caching
You can enable API caching in Amazon API Gateway to cache your endpoint's responses. With caching, you can reduce the number of calls made to your endpoint and also improve the latency of requests to your API.

### use case with lambda
API Gatway accepts the HTTP requests and routes it into a AWS Lambda function, which then returns a response to API Gateway, which then transforms it back to something the client wants.
