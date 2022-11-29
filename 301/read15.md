# Authentication

## What is OAuth

1. What is OAuth?

    - Open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.
2. Give an example of what using OAuth would look like.

    - Log on a website using other website's/service logon.
3. How does OAuth work? What are the steps that it takes to authenticate the user?

    1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
    2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
    3. The first site gives this token and secret to the initiating user’s client software.
    4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
    5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
    6. The user approves (or their software silently approves) a particular transaction type at the first website.
    7. The user is given an approved access token (notice it’s no longer a request token).
    8. The user gives the approved access token to the first website.
    9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
    10. The second website lets the first website access their site on behalf of the user.
    11. The user sees a successfully completed transaction occurring.
    12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).
4. What is OpenID?

    - OpenID serves as a single sign-in, vouching for the identities of users in other sites.

## Authorization and Authentication flows

1. What is the difference between authorization and authentication?

    - Authorization is for machines to long into other machines to get information on behalf of humans. Authentication just a human to prove who he is to a machine when logging in.
2. What is Authorization Code Flow?

    - Enables a client application to obtain authorized access to protected resources like web APIs.
3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

    - OpenId Connect flow is specifically designed to authenticate native or mobile application users.
4. What is Implicit Flow with Form Post?

    - For public clients, or apps that are unable to securely store client secrets. It offers a streamlined workflow if the app only needs an ID token to perform user authentication.
5. What is Client Credentials Flow?

    - For M2M applications, the system authenticates and authorizes the app rather than a user.
6. What is Device Authorization Flow?

    - With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text. To do this, device apps use the Device Authorization Flow (drafted in OAuth 2.0). For use with mobile/native applications.
7. What is Resource Owner Password Flow?

    - Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form. The Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used.

### Sources

- <https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html>
- <https://auth0.com/docs/get-started/authentication-and-authorization-flow>

[Back To Home](../README.md)
