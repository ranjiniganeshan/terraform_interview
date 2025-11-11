## Terraform interview questions

1. What does terraform init does ?

Backend Initialization: It sets up the backend where Terraform stores the “state” of your infrastructure, which is a record of managed resources and configuration.​

Provider Plugins: The command downloads and installs the provider plugins (like aws, azurerm, etc.) required to interact with cloud services, based on your configuration’s needs.​

Lock File Creation: terraform init generates a .terraform.lock.hcl file, which locks the provider versions used so that subsequent team members will use the same versions for consistency. This lock file should be added to version control.​

Module Initialization: If your configuration references remote modules, terraform init will download them so they’re ready to use.​

Configuration Validation: It checks your Terraform files for syntax and compatibility before other commands are executed.


## 
