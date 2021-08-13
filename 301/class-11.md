# Readings: Authentication

[Return to 301 TOC](301TOC.md)

## What is OAuth

**[Reading from - Link](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)**

- **What is OAuth?** > Open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credentials - source from article.

- **Give an example of what using OAuth would look like.** > You go to website "A" and it offers the ability to login using your Google info. By clicking on the login with Google option, Google will authenticate you and website "A" logs you on itself afterwards using the permission gained from Google.

- **How does OAuth work? What are the steps that it takes to authenticate the user?** > OAuth only works with HTTPS! Assuming the user is already signed into one website or service.

1. The first website connects to the second website on behalf of the user using OAuth, providing the user's verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first website gives this toek and secret to the initiating user's client software.
4. Client's software presents the request token and secret to their authorization provider.
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
6. The user approves (or their software silently approves) a particular transaction type at the first website.
7. The user is given an approved access token.
8. The user gives the approved access token to the first website.
9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
10. The second website lets the first website access their site on behalf of the user.
11. The user sees a successfully completed transaction occuring.

- **What is OpenID?** > OpenID is for authentication. Not popular but 2014 OpenID Connect was released which reinvented OpenID as an authentication layer for OAuth.

## Authorization and Authentication flows

**[Reading from - Link](https://auth0.com/docs/flows)**

- **What is the difference between authorization and authentication?** > Authentication is the process of verifying who a user is. Authorization is the process of verifying what they have access to.

- **What is Authorization Code Flow?** > Only used on servers where the source code is not publicly exposed. Exchanges an Authorization code for a token. Your app must be server-sdie because during this exchange, you must also pass along oyur application's Client Secret, which must also be kept secure and oyu will have to store it in your client.

- **What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?** > Additional security added to the Code Flow for SPA, mobile & native applications. It makes use of a ProofKey for Code Exchange.

- **What is Implicit Flow with Form Post?** > Alternative to Authorization Code Flow which is intended for public clients, or applications which are unable to securely store Client Secrets. Not best proactice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication.

- **What is Client Credentials Flow?** > Used for M2M machine-to-machine applications such as CLIs, daemons or services running on your back-end, the system authenticates and authorizes the app rather than a user.

- **What is Device Authorization Flow?** > Used for input-constrained devices that connect to the internet. Rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. SmartTVs, AppleTV and others use this.

- **What is Resource Owner Password Flow?** > Only for highly trusted applications which request that users provide credentials(username & password) typically using an interactive form. Only use when redirect-based flows cannot be used.

## Bookmark/Skim

**[AuthO for single page apps](https://auth0.com/docs/libraries/auth0-react)**

### Things I want to know more about

- OAuth/Auth0 and how all these work.
- React Bootstrap or some other types of style libraries (Tailwind).
- Better understaind of this programming method of functional programming.
- Material UI
- Next.JS
- React Ionics

[Return to 301 TOC](301TOC.md)

[Return to Main Page](../README.md)
