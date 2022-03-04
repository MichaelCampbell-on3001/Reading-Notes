## Authentication

### [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

1. What is OAuth? **Open-standard authorization protocol**
1. Give an example of what using OAuth would look like. **Signing into a site with google authentication**
1. How does OAuth work? What are the steps that it takes to authenticate the user? 
  **- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.**
  **- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.**
  **- The first site gives this token and secret to the initiating user’s client software.
  **- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
  **- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
  **- The user approves (or their software silently approves) a particular transaction type at the first website.
  **- The user is given an approved access token (notice it’s no longer a request token).
  **- The user gives the approved access token to the first website.
  **- The first website gives the access token to the second website as proof of authentication on behalf of the user.
  **- The second website lets the first website access their site on behalf of the user.
  **- The user sees a successfully completed transaction occurring.
OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).
1. What is OpenID?

### [Authorization and Authentication flows](https://auth0.com/docs/flows)

1. What is the difference between authorization and authentication?
1. What is Authorization Code Flow?
1. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
1. What is Implicit Flow with Form Post?
1. What is Client Credentials Flow?
1. What is Device Authorization Flow?
1. What is Resource Owner Password Flow?
