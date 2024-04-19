# oauth_vue
Desarrolla el componente de OAUTH donde muestres la consulta de datos de tu perfil de usuario de manera ordenada. Ya sea con el uso de una librería de CSS o con los datos ordenados.

## Logging In and Gated Content
This sample demonstrates:

Logging in to Auth0 using Redirect Mode
Accessing profile information that has been provided in the ID token
Gated content. The /profile route is not accessible without having first logged in
Project setup
## npm install
Configuration
The project needs to be configured with your Auth0 domain and client ID in order for the authentication flow to work.

To do this, first copy auth_config.json.example into a new file in the same folder called auth_config.json, and replace the values within with your own Auth0 application credentials:

{
  "domain": "<YOUR AUTH0 DOMAIN>",
  "clientId": "<YOUR AUTH0 CLIENT ID>"
}
Compiles and hot-reloads for development
npm run serve
Deployment
Compiles and minifies for production
npm run build
Docker build
To build and run the Docker image, run exec.sh, or exec.ps1 on Windows.

Lints and fixes files
npm run lint
What is Auth0?
Auth0 helps you to:

Add authentication with multiple authentication sources, either social like Google, Facebook, Microsoft Account, LinkedIn, GitHub, Twitter, Box, Salesforce, among others, or enterprise identity systems like Windows Azure AD, Google Apps, Active Directory, ADFS or any SAML Identity Provider.
Add authentication through more traditional username/password databases.
Add support for linking different user accounts with the same user.
Support for generating signed Json Web Tokens to call your APIs and flow the user identity securely.
Analytics of how, when and where users are logging in.
Pull data from other sources and add it to the user profile, through JavaScript rules.
Create a Free Auth0 Account
Go to Auth0 and click Sign Up.
Use Google, GitHub or Microsoft Account to login.
Issue Reporting
If you have found a bug or if you have a feature request, please report them at this repository issues section. Please do not report security vulnerabilities on the public GitHub issue tracker. The Responsible Disclosure Program details the procedure for disclosing security issues.


