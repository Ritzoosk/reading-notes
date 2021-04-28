## Correct order:
- Register your application to get a client_id and client_secret
- Ask the client if they want to sign in via a third party
- Redirect to a third party authentication endpoint
- Make a request to a third-party API endpoint
- Make a request to the access token endpoint
- Receive authorization code
- Receive access token


### What can you do with an authorization code?
- get into protected routes

### What can you do with an access token?
- get into a protected "account"

### What’s a benefit of using OAuth instead of your own basic authentication?
- enterprise level industry standard. Easy implamentation. allows cross application authorization.


## Terms
Client ID
 - public identifier, normally encoded
Client Secret
  - a chosen string that further encrypts your data
Authentication Endpoint
  - where you make auth requests
Access Token Endpoint
  - when your app goes to get a token
API Endpoint
  - 
Authorization Code
  - the hex code thats compared against the stored encrytped string 
Access Token
  - once auth is confirmed a token is issued


### Which 3 things had you heard about previously and now have better clarity on?
- Authorization headers, tokens, and "secret"
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- client ID, Endpoints
### What are you most excited about trying to implement or see how it works?
- access tokens!