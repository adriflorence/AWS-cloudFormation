# Infrastructure as Code

This is a basic setup of networking infrastructure as code based on a structure diagram.

## Components included:

- VPC
- Internet Gateway
- Subnets (2 x public, 2 x private)
- Route Table (1 x public, 2 x private)
- Route Table Associations

## Trigger stack update:

``` aws cloudformation update-stack --stack-name test --region us-west-2 --template-body file://infrastructure.yml --parameters file://parameters.json ```