# Create 4 ressources in Azure
### resource_group
### service_plan
### app_service
### app_service_auto_scale

# How to run Terraform:
### az login
### az account list --query "[][isDefault,id,name]" --output table
### az account set --subscription "xxxxx-xxxxx-xxxxx-xxxxx-xxxxx"
### terraform init
### terraform workspace new dev
### terraform validate -var-file="myVars.tfvars"
### terraform plan -var-file="myVars.tfvars" -out dev.tfplan
### terraform apply dev.tfplan

# How to clean up ressources from Azure
### terraform workspace select default
### terraform destroy -var-file="myvars.tfvars" -force
### terraform workspace delete dev
