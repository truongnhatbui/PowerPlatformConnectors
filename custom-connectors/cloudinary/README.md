## Cloudinary Connector

Cloudinary is a cloud service that offers a solution to a web application's entire image management pipeline.

## Prerequisites

You will need the following to proceed:

- A Microsoft Power Apps or Power Automate plan with custom connector feature
- A Cloudinary Account
- The Power Platform CLI tools

## Building the connector

Since the Cloudinary APIs are secured, you will need

1. Access to a Cloudinary instance
2. A user account on the Cloudinary Mangement Console [https://cloudinary.com/users/login](https://cloudinary.com/users/login)
3. An active Cloudinary API (also known as an API plan) and valid Cloudinary API credentials
   After that is completed, you can create and test the connector.

### Deploying the sample

Run the following commands and follow the prompts:

```paconn
paconn create --api-def apiDefinition.swagger.json --api-prop apiProperties.json
```

## Supported Actions

The connector supports the following actions:

- **Resources Operations**
  - `Get resources`: Lists resources (assets) uploaded to your account.
  - `Get resources by tag`: Lists resources (assets) with a specified tag. This method does not return deleted assets even if they have been backed up.
