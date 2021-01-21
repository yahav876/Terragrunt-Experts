Wellcome To my little terragrunt project !

In this project we are building a VERY DRY env with terraform via terragrunt.

* DRY remote state file
* DRY proivders
* REUSABLE Modules 

Stracture :

├── environments
│   ├── prod
│   │   └── test
│   ├── qa
│   │   └── test
│   └── stage
│       ├── acm
│       │   └── terragrunt.hcl
│       ├── ec2
│       │   └── terragrunt.hcl
│       ├── sec-group
│       │   └── terragrunt.hcl
│       ├── terragrunt.hcl
│       └── vpc
│           └── terragrunt.hcl
├── modules
│   ├── acm
│   │   ├── main.tf
│   │   ├── outputs.tf
│   │   └── variables.tf
│   ├── ec2
│   │   ├── ansible.cfg
│   │   ├── ansible-playbooks
│   │   │   ├── inventory_ansible
│   │   │   │   └── tf_aws_ec2.yml
│   │   │   ├── jenkins-master-sample.yaml
│   │   │   └── jenkins-worker-sample.yaml
│   │   ├── main.tf
│   │   ├── outputs.tf
│   │   └── variables.tf
│   ├── sec-group
│   │   ├── main.tf
│   │   ├── outputs.tf
│   │   └── varibales.tf
│   └── vpc
│       ├── main.tf
│       ├── outputs.tf
│       └── variables.tf
└── README.md


We are building here in the end env like this: 
