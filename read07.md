# Bearer Authorization

## Review, Research, and Discussion

1. Write the following steps in the correct order:

- Register your application to get a client_id and client_secret
- Ask the client if they want to sign in via a third party
  - (IF THEY WANT TO SIGN IN VIA 3RD PARTY OTHERWISE, SKIP) 
  - Redirect to a third party authentication endpoint 
  - Make a request to a third-party API endpoint
- Receive authorization code
- Make a request to the access token endpoint
- Receive access token


2. What can you do with an authorization code?

- you trade an authorizationg code for a authorization token, which grants users access to otherwise private/restricted data

3. What can you do with an access token?

- retrive and manupliate data than can only be accessed with a token

4. What’s a benefit of using OAuth instead of your own basic authentication?

- some benefits can be:
  - quick access and consolidated logins for websites
  - less login/passwords
  - transfer unique user data (fill out name forms, age, date of birth automatically)

## Terminology

- Client ID:
  - public identifier for apps

- Client Secret:
  - secret known only to the app and auth server

- Authentication Endpoint:
  - security measure to prevent unauthorized devices being able to connect to a network, site, or service

- Access Token Endpoint:
  - able to grant and verify an access token

- API Endpoint:
  - general communication between two systems

- Authorization Code:
  - temporary code or authorization that exchanges for an access token
  - obtained from authorization route/endpoint

- Access Token:
  - used in token based authentication which allows access to other routes/data that are otherwise restricted

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?

- Access tokens, Authentication Endpoint, and Oauth

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Really want to learn about Oauth, solidify the flow of creation of an account, and logging in and receiving a token

3. What are you most excited about trying to implement or see how it works?

- I want to build a fully functional app like twitter just to see if i can


## What is JWT ? JSON Web Token Explained

- JWTs are compact, they can be sent over URL easily
- JWTs are intended for use between any two parteis.
- JWT is an Open Standard

## Is JWT secure?

- if you don't know the secret, you can't modify the JWT

## References:

- https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/