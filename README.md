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


![image](https://github.com/user-attachments/assets/98037de3-7736-45f6-99b6-fabbe9e6add4)

Lets again create a new stack

$ aws cloudformation create-stack --stack-name cfn-workshop-resources --template-body file://resources.yaml
{
    "StackId": "arn:aws:cloudformation:us-east-1:157514729189:stack/cfn-workshop-resources/6a5b5e50-d51f-11ef-8bde-0edb2933a48b"
}

![image](https://github.com/user-attachments/assets/41895be7-9a96-412f-bf65-786e384e86cb)

# Intrinsic functions
Intrinsic functions are built-in functions that help you manage your stacks. Without them, you will be limited to very basic templates
