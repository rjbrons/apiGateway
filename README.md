# apiGateway

Let’s use Lambda to expose our repeated-word-in-sentence functionality to the world!

## API
make a GET request to this route with ?input={some string} at the end to receive a response with the first repeated word.  
`https://281k8c1ic5.execute-api.us-east-2.amazonaws.com/repeatedWord/repeatedWords`

Note: the function IS case sensitive, ie. It and it are different words.

## Issues
- the UI for API Gateway is bonkers.
- somehow the URL for the endpoint changes after you hit it once, so I had issues with auth token unless I copied and pasted the URL directly into the browser and added the query string to it.
- understanding how to create a mapping for the input params from json to a string - or what we ended up doing and pulling the string out of the json KVP.
