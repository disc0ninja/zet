# Terraform

Tool that can be used locally or in the cloud for building, changing, and versioning infrastructure.

## Key Features
- Infrastructure as code. Written in Terraform Configuration Language
- Execution Plans: Helps avoid surprises when depolying configurations.
- Resource Graph: Terraform builds a graph of all yourn resources and gives insight into the creation and modification of resources.
- Change Automation: The combination of the resource graph and execution plans, help reduce human error and allow you to know **exactly** what will change, and in what order.

## Key Files
- **terraform_config.tf**: Primary configuration file and can be (and likely is) split into multiple files, that *Terraform* combines into a single file before applying it.  
- **terraform.tfvars**: Input variables. Allows aspects of the midule ot be customized without changing the module source code.
- **terraform.tfstate**: A snapshot of a successfully applied *Terraform* configuration.

## Resources
- [tfenv](https://github.com/disc0ninja/zet/search?q=tfenv) is a *Terraform* version manager <https://github.com/tfutils/tfenv>  
- Docs <https://terraform.io/docs/index.html>

