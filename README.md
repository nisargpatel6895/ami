# ami

- A new user circleci is created in AWS IAM services.
- Using circleci access key and secret key we build AMI Image in AWS by configurations mentioned in ubuntu-ami.json

There are two workflows in CI/CD pipeline to build AMIs
 1. To validate packer
 - packer validate -var-file=variables.json ubuntu-ami.json

 2. To build AMI with packer
 - packer build -var-file=variables.json ubuntu-ami.json