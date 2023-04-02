[View code on GitHub](https://dune.com/docs/api/api-reference/authentication.md)

The app technical guide titled "Authentication" provides instructions on how to authenticate API requests in the Dune app. The guide emphasizes the importance of API keys in determining the permissions of private queries and billing for requests. It warns against sharing secret API keys in publicly accessible areas to ensure security.

The guide provides a specific method for authenticating requests, which involves adding an "x-dune-api-key" property to the request header. This property is required for all request types. The guide includes an example of how to do this with an Execute POST API request using the curl command:

```
curl -X POST -H x-dune-api-key:{{api_key}} "https://api.dune.com/api/v1/query/{{query_id}}/execute"
```

Overall, this guide is essential for developers working on the Dune app who need to authenticate API requests. It provides clear instructions on how to do so and emphasizes the importance of keeping API keys secure.
## Questions: 
 1. What type of authentication does the Dune API use?
- The Dune API uses API keys to authenticate requests.

2. What is the purpose of the "x-dune-api-key" property in the request header?
- The "x-dune-api-key" property is used for authentication with the API and is needed on all request types.

3. What is the recommended practice for handling secret API keys?
- The recommended practice is to not share secret API keys in publicly accessible areas such as GitHub or client-side code.