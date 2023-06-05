
## What is OAuth?

[Source](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

1. Give an example of what using OAuth would look like. It's when you can sign into one OAuth provider to login into a separate OAuth provider. OAuth providers include Google, GitHub, Facebook, etc.

2. How does OAuth work? OAuth authenticates the user during the initial login on the first site and exchanges tokens with subsequent OAuth providers in order to gain authorization for access to the resources on subsequent providers.

What are the steps that it takes to authenticate the user?

**Step One:** First OAuth site connects to second site using the verified identification/credentials during the initial connection to first OAuth site

**Step Two** The second OAuth site generates a single-use token and secret unique to the transaction and parties involved.

**Step Three** *The first site gives this token and secret to the initiating user’s client software.
The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).*

*If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
The user approves (or their software silently approves) a particular transaction type at the first website.*

**Step Four** The user is provided an approved access token and sends the token to the first website.

**Step Five** The first OAuth site passes this token to second OAuth site *as proof of authentication on behalf of the user.* and then proceeds to let *the second website lets the first website access their site on behalf of the user.* And the authorization transaction is complete.

3. What is OpenID? This one is based on the concept of open authentication where 

## Authorization and Authentication flows

[Source](https://auth0.com/docs/get-started/authentication-and-authorization-flow)

1. What is the difference between authorization and authentication? Authorization is about gaining access to resources and authentication is about confirming owner of same resources

2. What is Authorization Code Flow? *involves exchange of authorization code for an access token

![Image](Screenshot%202023-06-05%20at%204.47.38%20PM.png)

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

This uses an additional layer of security on the Authorization Code Flow through use of Code Verifier and Code Challenge

![Image](Screenshot%202023-06-05%20at%204.51.18%20PM.png)

4. What is Implicit Flow with Form Post? 

Looks like this uses an ID token and is not as secure as the other ones

![Image](Screenshot%202023-06-05%20at%204.55.35%20PM.png)

5. What is Client Credentials Flow?
 
 It involves applications exhanging application credentials for access token

![Image](Screenshot%202023-06-05%20at%204.59.05%20PM.png)

6. What is Device Authorization Flow?

Asks the user to authorize from a device tied to user credentials

![Image](Screenshot%202023-06-05%20at%205.00.53%20PM.png)

7. What is Resource Owner Password Flow?

Credentials are stored and sent to the backend, must only use if user trusts application. This one is not very secure. 

![Image](Screenshot%202023-06-05%20at%205.03.51%20PM.png)

Bookmark and Review
[Auth0 for single page apps](https://auth0.com/docs/libraries/auth0-react)