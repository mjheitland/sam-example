# Deploy Lambda Function with SAM

sam package \
--template-file template.yaml \
--output-template-file packaged.yaml \
--s3-bucket heitlm-094033154904-eu-west-1

sam deploy \
--region eu-west-1 \
--template-file ~/dev/sam-example/packaged.yaml \
--capabilities CAPABILITY_IAM \
--stack-name sam-example-1

sam delete-stack \
--region eu-west-1 \
--stack-name sam-example-1
