---
sidebar_position: 2
sidebar_label: "Quick Start"
---

# Getting Started

Get started by **creating a new Keyp app**.

1. Create a Keyp App in the developer portal
2. Use an OAuth2.0 library to authenticate users (eg. Passport.js)
3. Use the API endpoints to airdrop tokens to your users

## Creating a developer account

Log in to https://dev.UseKeyp.com and sign-in with Google, Discord, or your Chess.com account.

![Login Page](/img/dev-portal-login-page.png)

## Getting an App ID

On your developer profile page, select "Create Client", which will create a new Keyp App, and provide the credentials `Client Id`. You can create as many clients as you would like.

![Client Generation](/img/dev-portal-client-gen.gif)

## Connecting Keyp to your application

Keyp works like other social login providers, using OAuth2.0 to authenticate and give access to user accounts. You can also skip this step and start using the API immediately.

You can do this using any application framework (React, Node, Express...) or language (JS, Python, Go, Unity...). Here is just a sample of the many libraries available to use:

- Passport.js [passport-oauth2](https://www.passportjs.org/packages/passport-oauth2/)

We created a few example Keyp Apps, which you can use to get started:

- **ExpressJS** - [usekeyp-example-app-express](https://github.com/UseKeyp/usekeyp-example-app-express/)
- **RedwoodJS** - [usekeyp-example-app-redwood](https://github.com/UseKeyp/usekeyp-example-app-redwood/)

Learn more in the [OAuth](/oauth) section.

## Using the API to move tokens

With a user's _access token_, you can see info about their account, and make certain transactions they've authorized.

To test immediately, copy the Access Token

![Access Token](/img/dev-portal-access-token.png)

To help you test the API, we created a Postman Workspace:

[Keyp Public Workspace](https://www.postman.com/speeding-spaceship-663022/workspace/keyp-public-workspace/collection/25667367-e1156fb2-60c3-4a42-b76b-47902a22512e?ctx=documentation)

All you need is your acc
