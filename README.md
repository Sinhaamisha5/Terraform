# Terraform
My terraform code
$ aws ec2 describe-vpcs --filters Name=isDefault,Values=true --query "Vpcs[].VpcId" --region us-east-1
[
    "vpc-077622373e3b8f313"
]

Create a stack
$ aws cloudformation create-stack --stack-name cnf-workshop-template-and-stack --template-body file://template-and-stack.yaml
{
    "StackId": "arn:aws:cloudformation:us-east-1:157514729189:stack/cnf-workshop-template-and-stack/1da3fdc0-d519-11ef-bc18-0e6906661d7d"
}

update a stack
$ aws cloudformation update-stack --stack-name cnf-workshop-template-and-stack --template-body file://template-and-stack.yaml

Delete a stick
$ aws cloudformation delete-stack --stack-name cnf-workshop-template-and-stack

![image](https://github.com/user-attachments/assets/8772b9a8-5c35-4055-96b2-41f11b51ad07)
