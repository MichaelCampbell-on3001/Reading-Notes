## Authentication

### [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

1. What is OAuth? **Open-standard authorization protocol**
1. Give an example of what using OAuth would look like. **Signing into a site with google authentication**
1. How does OAuth work? What are the steps that it takes to authenticate the user? 
  **- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.**
  
  **- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.**
  
  **- The first site gives this token and secret to the initiating user’s client software.**
  
  **- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).**
  
  **- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.**
  
  **- The user approves (or their software silently approves) a particular transaction type at the first website.**
  
  **- The user is given an approved access token (notice it’s no longer a request token).**
  
  **- The user gives the approved access token to the first website.**
  
  **- The first website gives the access token to the second website as proof of authentication on behalf of the user.**
  
  **- The second website lets the first website access their site on behalf of the user.**
  
  **- The user sees a successfully completed transaction occurring.**

1. What is OpenID? **allows you to use an existing account to sign in to multiple websites, without needing to create new passwords.**

### [Authorization and Authentication flows](https://auth0.com/docs/flows)

1. What is the difference between authorization and authentication? **authentication is the process of verifying who someone is, whereas authorization is the process of verifying what specific applications, files, and data a user has access to.**
1. What is Authorization Code Flow? **exchanges an Authorization Code for a token**
1. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)? **It is used during authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Additionally, single-page apps have special challenges.**
1. What is Implicit Flow with Form Post? **It is intended for Public Clients, or applications which are unable to securely store Client Secrets.**
1. What is Client Credentials Flow? **When the system authenticates and authorizes the app rather than a user.**
1. What is Device Authorization Flow? **rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device.**
1. What is Resource Owner Password Flow? **It requests that users provide credentials (username and password), typically using an interactive form.**
