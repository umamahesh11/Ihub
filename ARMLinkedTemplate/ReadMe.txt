az deployment group create \
  --name deploymentName\
  --resource-group ResourcegroupName \
  --template-uri "https://mystorageaccountjk.blob.core.windows.net/jklinkedtemplates/main.json"\
  --parameters "https://mystorageaccountjk.blob.core.windows.net/jklinkedtemplates/main-template-parameter.json"


##################
Put 1) template-uri =  url of main template file.
    2) parameters = url of parameter file of main template file 

##################
KeyVault Secrete Configurations:
    Update KeyVault parameters in below files:
    1) database-parameter.json
    2) vnet.parameters.json    