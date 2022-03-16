# Costs to Expect API: Documentation

## Self-documenting

We have tried to make our API as easy to use as possible, although our documenation is thorough, our goal is you don't read it, once you have fetched the resposne for the root of the API, you should be able to get at anything you need.

## OPTIONS requests

We have added an OPTIONS endpoint for every route, the OPTIONS request reponse will will list the endpoints supported by the route, any parameters and fields as well as a general overview of the purpose.

## Summaries

If a summary route exists for a collection, the summary route will always by the route with a `/summary/` prefix. A summary route will support all the same parameters as as the collection it summarises.

## Cache

All collections and summaries are cached, if you would like to override the cache and fetch fresh data, include the `X-Skip-Cache` header. The value of the header does not matter

## Public data

The Costs to Expect API includes public data, if you don't want to see any public data, include `exclude-public=1` in any request URIs.

## Responses

Collections will return an array and a 200.

Items will return a single object and a 200.

A successful POST request will return a single object and a 201.

A successful PATCH request will return 204.

A successful DELETE request will return a 204.

Non 2xx results will return an object with a message field and optionally a fields array.

A validation error will return a 422, the response will include a fields array containing all the validation errors.

## Caching

We include local level caching in the API, as time goes on we will move towards conditional caching, specifically including an Etag header and returning a 304 response.

## Headers

Responses will include multiple headers, the table below details the intention behind each of our custom headers.

| Header          | Purpose                                                      |
| :-------------- | :----------------------------------------------------------- |
| X-Total-Count   | Pagination: Total number of result                           |
| X-Count         | Pagination: Number of results returned                       |
| X-Limit         | Pagination: Limit value applied to request after validation  |
| X-Offset        | Pagination: Offset value applied to request after validation |
| X-Offset        | Pagination: Offset value applied to request after validation |
| X-Link-Previous | Pagination: URI for previous result set if relevant          |
| X-Link-Next     | Pagination: URI for next result set if relevant              |
| X-Link-Next     | Pagination: URI for next result set if relevant              |
| X-Last-Updated  | The last time the collection was updated                     |
| X-Sort          | Sort options applied to request after validation             |
| X-Search        | Search options applied to request after validation           |
| X-Parameters    | Request parameters applied to request after validation       |
