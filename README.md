# Kinde Starter Kit - Java

This is a Java template with [KindeAuth](https://kinde.com/docs/developer-tools/java-sdk/).

## Register an account on Kinde

To get started set up an account on [Kinde](https://app.kinde.com/register).

## Setup your local environment

Clone this repo and install dependencies by running `mvn clean install`

In `application.properties` file, set the following variables with the details from the Kinde `App Keys` page

> kinde.host - The token host value
>
> kinde.client.secret - The client secret

e.g

```
kinde.host=https://<your_subdomain>.kinde.com
kinde.client.secret=<your_client_secret>
```

## Set your Callback and Logout URLs

Your user will be redirected to Kinde to authenticate. After they have logged in or registered they will be redirected back to your Java application.

You need to specify in Kinde which url you would like your user to be redirected to in order to authenticate your app.

On the App Keys page set ` Allowed callback URLs` to `http://localhost:8080/api/auth/kinde_callback`

> Important! This is required for your users to successfully log in to your app.

You will also need to set the url they will be redirected to upon logout. Set the `Allowed logout redirect URLs` to http://localhost:8080.

## Start the app

Run project and navigate to `http://localhost:8080`.

Click on `Sign up` and register your first user for your business!

## View users in Kinde

If you navigate to the "Users" page within Kinde you will see your newly registered user there. 🚀