# Terraform

## Make sure you're in the project directory with the .tf files

## Make sure that you are log into AWS (aws configure) and AZ (az login)

```bash
#initiate, review, deploy, destroy
terraform init

terraform plan

terraform apply -auto-approve

terraform destroy -auto-approve

#get IP and connect
ssh -i ~/.ssh/id_ed25519 azureuser@$(terraform output -raw public_ip)

#recycle just the VM later
terraform destroy -target azurerm_linux_virtual_machine.vm

```
