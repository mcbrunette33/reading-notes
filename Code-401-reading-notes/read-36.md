## Read 36

- The Auth category can be used to register a user, confirm attributes like email/phone, and sign in with optional multi-factor authentication. It is set up to use Amazon Cognito User Pools which manages the users and their properties.

- The default CLI flow as mentioned in the getting started guide requires a username, password and a valid email id as parameters to register a user. Invoke the following api to initiate a sign up flow.

- The next step in the sign up flow is to confirm the user. A confirmation code will be sent to the email id provided during sign up. Enter the confirmation code received via email in the confirmSignUp call.

- Implement a UI to get the username and password from the user. After the user enters the username and password you can start the sign in flow by calling the following method:

- If you create or update an SMS MFA configuration for your Cognito user pool, the Cognito service will send a test SMS message to an internal number in order to verify your configuration. You will be charged for these test messages by Amazon SNS.
For information about Amazon SNS pricing, see Worldwide SMS Pricing.

- Note that you must call confirmSignIn in the same app session as you call signIn. If you close the app, you'll need to call signIn again. As a result, for testing purposes, you'll at least need an input field where you can enter the code sent via SMS and feed it to confirmSignIn.
