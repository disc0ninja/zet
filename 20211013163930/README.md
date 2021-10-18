# Terraform Variables Functions and Modules

## Modules 
- Do not support *counts* like variables do, and must be added by hand.
 
## Variables 
- Name 
- type (Optional) 
- default (Optional) 

- Can have multiple sources which are *overriding* 
Below are the sources are listed in order of precedence. (e.g Command Line will overwrite a variable set in a file.)
  1. Command line
  1. File 
  1. Environment 
 
``` 
# Specify default variable and type 
variable "variable_name" { 
  type = string 
  default = "development" 
} 
```
```
# specify variable in file 
variable_name = "dev"
```
```
# specify variable in-line
terraform plan -var 'variable_name=dev'
```
