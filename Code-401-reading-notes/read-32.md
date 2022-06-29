## Read 32

- Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers

- Serverless applications are event-driven cloud-based systems where application development rely solely on a combination of third-party services, client-side logic and cloud-hosted remote procedure calls

- Eamples of serverless clouds ( AWS Lambda, Google Cloud Functions, Azure Functions, IBM OpenWhisk, Alibaba Function Compute, Iron Functions, Auth0, Webtask, Oracle Fn Project, Kubeless)

- Scaling process for Serverless is automatic and seamless, but there is a lack of control or entire absence of control. While automatic scaling is great, it’s difficult not to be able to address and mitigate errors related to new Serverless instances.

- FaaS is an implementation of Serverless architectures where engineers can deploy an individual function or a piece of business logic.

- AWS Amplify is a set of purpose-built tools and features that lets frontend web and mobile developers quickly and easily build full-stack applications on AWS, with the flexibility to leverage the breadth of AWS services as your use cases evolve. With Amplify, you can configure a web or mobile app backend, connect your app in minutes, visually build a web frontend UI, and easily manage app content outside the AWS console. Ship faster and scale effortlessly—with no cloud expertise needed.

- The Amplify CLI generates the Todo database table upon amplify push and generates a GraphQL API to perform create, read, update, delete, and list operations for the Todo model.

- Every GraphQL type with the @model directive will automatically have an id field set as the primary key. You can override this behavior by marking another required field with the @primaryKey directive.

- Amplify uses Amazon DynamoDB tables as the underlying data source for @model types. For key-value databases, it is critical to model your access patterns with "secondary indexes". Use the @index directive to configure a secondary index.

- Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale but making it work for your access patterns requires a bit of forethought. 

- DynamoDB query operations may use at most two attributes to efficiently query data.