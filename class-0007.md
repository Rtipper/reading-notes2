# Class 7 Reading Notes

### 1. Review, Research, and Discussion
#### Write the following steps in the correct order:
- Register your application to get a client_id and client_secret
- Ask the client if they want to sign in via a third party
- Redirect to a third party authentication endpoint
- Receive authorization code
- Make a request to the access token endpoint
- Receive access token
- Make a request to a third-party API endpoint

### 2. What can you do with an authorization code?
- With an authorization code, you can allow a user to acces specific pages, information or privileges throughout your web application. i.e. administrator/mod privileges, editing rights, delete/add content, access specific web pages etc.

### 3. What can you do with an access token?
- An access token, much like entering a token at good ol Chuck E Cheese, allows you to access specificlly requested things, such as APIs, routes or any other part of the site that requires permission to access.

### 4. What’s a benefit of using OAuth instead of your own basic authentication?
- Much more in-depth and ethical way of encrypting user information when they sign-up for your web app as well as making the coding process easier on yourself as a dev and them as a user.

### VOCAB
- Client ID: a public identifier for apps
- Client Secret: a secret known only to the application and the authorization server
- Authentication Endpoint: the route in which authentication occurs
- Access Token Endpoint: is used by the application in order to get an access token or a refresh token
- API Endpoint: the point of entry in a communication channel when two systems are interacting -- refers to touchpoints of the communication between an API and a server.
- Authorization Code: an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space.
- Access Token: an object encapsulating the security identity of a process or thread -- used to make security decisions and to store tamper-proof information about some system entity.

#### REFS:
- https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/
- https://auth0.com/docs/protocols/protocol-oauth2
