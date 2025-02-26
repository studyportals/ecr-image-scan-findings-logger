# Logging image scan findings from Amazon ECR in CloudWatch using an AWS Lambda function

Steps to create the solution:

1. Download the [Template-ECR-SFL.yml](Template-ECR-SFL.yml) template.
2. Upload the template to CloudFormation and create a new stack.
3. Test the solution by scanning an image on ECR. Then, go to CloudWatch and check log groups starting with ‘/aws/ecr/image-scan-findings/repository name’.
4. Feel free to modify the Lambda function code within the template and/or create the resources manually.

## ⚠️ Important 
Stack tags cannot be directly implemented within the template. \
If creating a new stack is necessary, ensure to add the following tags during the `Configure stack options` step, as specified in [Tag Definition](https://knowledge-vault.studyportals.xyz/manuals/aws/tagging-policy.html#tag-definitions)