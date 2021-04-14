<table><tbody><tr><td valign="center"><img src="https://lh3.googleusercontent.com/kWMH3aQzcvLmucr5wIL-2BlmiFDgQgiB-fCS6J2Du7H-T1zL3rWP7JU2Om81dIkStE3mP6cLYt1fhCCIPHY6RYMpUg7oRphN11bCz--0Mv4PrsrhfrmdMurdt2XeEYbUKvqYnrj-" align="left" width="250"></td><td valign="center"> This project is deprecated and is no longer being actively being actively maintained. </td></tr></tbody></table>

Please see the [accept a payment](https://github.com/stripe-samples/accept-a-payment) sample showing how to accept Card payments and more payment method types with React Stripe.js.


# Card Payment using React

This sample shows how to build a card form to take a payment using the [Payment Intents API](https://stripe.com/docs/payments/payment-intents), [Stripe Elements](https://stripe.com/payments/elements) and [React](https://reactjs.org/).

See a hosted version of the [demo](https://rl6zb.sse.codesandbox.io/) in test mode or [fork on codesandbox.io](https://codesandbox.io/s/github/stripe-samples/react-elements-card-payment/tree/codesandbox)

<img src="./demo.png" alt="Preview of recipe" align="center">

## Features

This sample consists of a `client` in React and a `server` piece available in 5 common languages.

The client is implemented using `create-react-app` to provide the boilerplate for React. Stripe Elements is integrated using [`react-stripe-js`](https://github.com/stripe/react-stripe-js), which is the official React library provided by Stripe.

The server includes [5 server implementations](server/README.md) in Node, Ruby, Python, Java, and PHP in the [/server](/server) directory. We included several RESTful server implementations, each with the same endpoints and logic.

## How to run locally

To run this sample locally you need to start both a local dev server for the `front-end` and another server for the `back-end`.

You will need a Stripe account with its own set of [API keys](https://stripe.com/docs/development#api-keys).

Follow the steps below to run locally.

**1. Clone and configure the sample**

The Stripe CLI is the fastest way to clone and configure a sample to run locally.

**Using the Stripe CLI**

If you haven't already installed the CLI, follow the [installation steps](https://github.com/stripe/stripe-cli#installation) in the project README. The CLI is useful for cloning samples and locally testing webhooks and Stripe integrations.

In your terminal shell, run the Stripe CLI command to clone the sample:

```
stripe samples create react-elements-card-payment
```

The CLI will walk you through picking your integration type, server and client languages, and configuring your .env config file with your Stripe API keys.

**Installing and cloning manually**

If you do not want to use the Stripe CLI, you can manually clone and configure the sample yourself:

```
git clone https://github.com/stripe-samples/react-elements-card-payment
```

Copy the .env.example file into a file named .env in the folder of the server you want to use. For example:

```
cp .env.example server/node/.env
```

You will need a Stripe account in order to run the demo. Once you set up your account, go to the Stripe [developer dashboard](https://stripe.com/docs/development/quickstart#api-keys) to find your API keys.

```
STRIPE_PUBLISHABLE_KEY=<replace-with-your-publishable-key>
STRIPE_SECRET_KEY=<replace-with-your-secret-key>
```

### Running the API server

1. Go to `/server`
1. Pick the language you are most comfortable in and follow the instructions in the directory on how to run.

### Running the React client

1. Go to `/client`
1. Run `yarn`
1. Run `yarn start` and your default browser should now open with the front-end being served from `http://localhost:3000/`.

### Using the sample app

When running both servers, you are now ready to use the app running in [http://localhost:3000](http://localhost:3000).

1. Enter your name and card details
1. Hit "Pay"
1. 🎉

## FAQ

Q: Why did you pick these frameworks?

A: We chose the most minimal framework to convey the key Stripe calls and concepts you need to understand. These demos are meant as an educational tool that helps you roadmap how to integrate Stripe within your own system independent of the framework.

## Get support
If you found a bug or want to suggest a new [feature/use case/sample], please [file an issue](../../issues).

If you have questions, comments, or need help with code, we're here to help:
- on [IRC via freenode](https://webchat.freenode.net/?channel=#stripe)
- on Twitter at [@StripeDev](https://twitter.com/StripeDev)
- on Stack Overflow at the [stripe-payments](https://stackoverflow.com/tags/stripe-payments/info) tag
- by [email](mailto:support+github@stripe.com)

Sign up to [stay updated with developer news](https://go.stripe.global/dev-digest).

## Author(s)

[@auchenberg-stripe](https://twitter.com/auchenberg)
