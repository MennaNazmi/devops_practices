# Day3 create VM using CLI

```
az group list -o table  


az vm create   --resource-group kml_rg_main-01436af0fe3348b1  --name devops-vm   --image Ubuntu2204   --size Standard_B2s   --admin-username azureuser  --generate-ssh-keys   --storage-sku Standard_LRS   --os-disk-size-gb 30

  ```