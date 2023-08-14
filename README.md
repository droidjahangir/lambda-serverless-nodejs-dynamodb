## steps :

1. Install serverless globally
```
npm install -g serverless
```

2. create AWS IAM user for serverless
create an user then copy `access key id` and secret access 

3. config serverless project
serverless documentation > cli reference > configuration

```
serverless config credentials --provider aws --key 1234 --secret 5678
```

4. verify configuration
need to open `~/.aws` then open credentials file to verify configurations

5. create nodejs project using serverless command
```
serverless create --template aws-nodejs
```

6. initiate package.json file using this command
```
npm init -y
```

7. After creating api we need to deploy 
```
sls deploy
```

**AWS CloudFormation dynamoDB user guide**
https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-dynamodb-table.html


**AWS javascript dynamodb sdk**
https://docs.aws.amazon.com/sdk-for-javascript/v3/developer-guide/dynamodb-examples-using-tables.html


**Install dependency**
```
npm install aws-sdk aws-jwt-verify
```

dev dependency
```
npm install --save-dev serverless-iam-roles-per-function
```

**see build file configuration definitions from this link**
https://docs.aws.amazon.com/codebuild/latest/userguide/build-spec-ref.html

**create artifact from this command**
```
serverless package --package my-artifact
```

### update github workflow from github actions marketplace

https://github.com/marketplace/actions/serverless


