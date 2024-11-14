# azure

1 - install Azure CLI

2 - install Terraform

    https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli 

3 - Create Service Principal and config environment

    https://developer.hashicorp.com/terraform/tutorials/azure-get-started/azure-build 

4 - Create a Azure Service Principal and export Terraform environment

    az ad sp create-for-rbac --role="Contributor" --scopes="/subscriptions/<SUBSCRIPTION_ID>"
    
    az login --service-principal -u <CLIENT_ID> -p <CLIENT_SECRET> --tenant <TENANT_ID>
    
    export ARM_CLIENT_ID="<appId>"
    
    export ARM_CLIENT_SECRET="<password>"
    
    export ARM_SUBSCRIPTION_ID="<SUBSCRIPTION_ID>"
    
    export ARM_TENANT_ID="<tenant>"

4 - Terraform commands

    terraform init 

    terraform fmt

    terraform validate

    terraform plan

    terraform apply

    terraform show
