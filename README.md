[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)

# Rails Authentication and Sessions

## Devise

https://github.com/plataformatec/devise

Devise is a flexible authentication solution for Rails based on Warden. It:

- Is a complete MVC solution based on Rails engines;
- Allows you to have multiple models signed in at the same time;
- Is based on a modularity concept: use only what you really need.

It's composed of 10 modules:

- Database Authenticatable: hashes and stores a password in the database to validate the authenticity of a user while signing in. The authentication can be done both through POST requests or HTTP Basic Authentication.

- Omniauthable: adds OmniAuth (https://github.com/omniauth/omniauth) support.

- Confirmable: sends emails with confirmation instructions and verifies whether an account is already confirmed during sign in.

- Recoverable: resets the user password and sends reset instructions.

- Registerable: handles signing up users through a registration process, also allowing them to edit and destroy their account.

- Rememberable: manages generating and clearing a token for remembering the user from a saved cookie.

- Trackable: tracks sign in count, timestamps and IP address.

- Timeoutable: expires sessions that have not been active in a specified period of time.

- Validatable: provides validations of email and password. It's optional and can be customized, so you're able to define your own validations.

- Lockable: locks an account after a specified number of failed sign-in attempts. Can unlock via email or after a specified time period

We will practice using documentation today and use the devise documentation as our guide for this lesson

- https://github.com/plataformatec/devise#getting-started
