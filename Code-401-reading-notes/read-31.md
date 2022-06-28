## Read 31

- AWS Amplify is a powerful toolkit developers use to build full stack applications that directly integrate with the cloud. Using it, developers can rapidly setup, test, launch, and scale production ready applications with minimal time spent focusing on the details.

- AWS Amplify is a toolchain that helps you build and deploy entire applications very quickly. Typically, this Amplify is mainly aimed at full stack applications, but you can also use it just for its ability to generate a backend.

-  we primarily use AWS Amplify as a Command Line Interface or CLI tool, however, there is a limited feature UI that allows you to do some administration tasks for some day to day activities

- Now the main strength of Amplify is that it quickly lets you add thigs like Storage, Authentication, Monitoring, and PubSub functionalities

- Amplify is an attractive tool because it allows developers to add application functionality without having to know what AWS services to use to achieve that functionality. This way, developers can spend more of their time focusing on application code as opposed to fumbling with infrastructure, deployment pipelines, and scaling considerations.

-  CloudFormation is an Infrastructure as Code service that allows you to define template files that instruct AWS which components you need for your application, and let AWS do the heavy lifting of provisioning those services.

###Amplify Features

- Authentication and Authorization, we rely on Amazon Cognito.

- To host APIs, either GraphQL or REST/HTTP based, we use either AWS Appsync or API Gateway, respectively.

- For raw object storage including asset files for your web applications, or deployment executables, we rely on the popular Amazon S3.

- For asynchronously communicate with other microservices, aka PubSub, we use a combination of Amazon Simple Notification Service (SNS) and Simple Queue Service (SQS).

- For analytics, we utilize Amazon Pinpoint.

- For domain registration and DNS modifications, we use Amazon Route 53.

- To build dashboards, examine logs, and add alarms we use Amazon Cloudwatch.

- For Serverless Compute we use AWS Lambda.

- And finally, for DataStores, we generally rely on the popular NoSQL Database Amazon DynamoDB.

