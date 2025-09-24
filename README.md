# Terraform

```bash
Make sure that you are log into AWS (aws configure) and AZ (az login)
```

```bash
#initiate, review, deploy, destroy
terraform init

terraform plan

terraform apply

terraform destroy

#get IP and connect
ssh -i ~/.ssh/id_ed25519 azureuser@$(terraform output -raw public_ip)

#recycle just the VM later
terraform destroy -target azurerm_linux_virtual_machine.vm

```
