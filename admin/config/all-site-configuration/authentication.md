---
description: Configure your user log-in options.
---

# Authentication

### Invite Only Mode

Check this option if you'd like your Forem to be private.  The only way that people will be able to create an account is [if you send them an invite](../../users/inviting-a-new-user.md).

### Authentication Methods

At this point, you can choose to enable any/all of:

* GitHub
* Twitter
* Facebook

### Email and Password

You can configure whether community members can use email/password to register and/or login.

### Generating Keys

Choose which authentication providers users can log in from. We currently offer:

* Twitter
  * [More info here](https://docs.forem.com/backend/auth-twitter/)
  * First, apply for a developer account at [developer.twitter.com](http://developer.twitter.com/) \(the approval process normally takes about a day\)
  * Then, [follow these instructions](https://developer.twitter.com/en/docs/authentication/guides/log-in-with-twitter) to generate the keys.
  * Callback URLs:
    * `https://{forem-url.com}/users/auth`
    * `https://{forem-url.com}/users/auth/twitter`
    * `https://{forem-url.com}/users/auth/twitter/callback`
    * `https://www.{forem-url.com}/users/auth`
    * `https://www.{forem-url.com}/users/auth/twitter`
    * `https://www.{forem-url.com}/users/auth/twitter/callback`
* [GitHub OAuth instructions](https://docs.github.com/en/developers/apps/creating-an-oauth-app)
  * [More information here](https://docs.forem.com/backend/auth-github/)
  * Callback URL: `https://{your-forem-url.com}/users/auth/github`
* [Facebook OAuth instructions](https://developers.facebook.com/docs/apps)
  * [More information here](https://docs.forem.com/backend/auth-facebook/) 

Apple and Google are coming soon.

In order to use these providers, you need to add their respective keys. You can create keys for these providers by visiting their developer portals, linked above.

