# Day2 
Create VM 
az vm create
–resource-group kml_rg_main-a79081730a6744fa
–name nautilus-vm
–image Ubuntu2204
–size Standard_B2s
–admin-username azureuser
–generate-ssh-keys
–os-disk-size-gb 30
–storage-sku Standard_LRS