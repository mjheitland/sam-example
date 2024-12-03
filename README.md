# Deploy API Gateway with Lambda Function using SAM

[Source](https://serverlessland.com/patterns/alb-lambda-rest-api-sam-py)

## Deployment

```bash
export AWS_REGION=eu-central-1
export AWS_DEFAULT_REGION=eu-central-1
export AWS_DEFAULT_PROFILE=mjheitland

sam validate

sam build

sam deploy --guided
```

## Teardown

sam delete