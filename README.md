# example-aws-s3-lambda
Example project for configuring a lambda to be triggered when a file is added to an S3 bucket.

## Prerequisites

Ensure the following AWS CLI's are installed.

[AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html)

[SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)

[Yarn Package Manager](https://yarnpkg.com/lang/en/)

This example referrs to an S3 bucket named `example-aws-s3-lambda` you will need to create your own S3 bucket and substitute your bucket name for the one this example uses. You can create a new S3 bucket on the command line using this command:

```
aws s3 mb s3://your-bucket-name
```

Please create your bucket and replace the two references to `example-aws-s3-lambda` in the `package.json` file.

## Install the Cloud Formation Stack

1. Package the stack.
	```
	yarn package
	```
2. Deploy the stack.
	```
	yarn deploy
	```


