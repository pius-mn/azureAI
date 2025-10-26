## MLS files for CI/CD project
projectName="MLOPS17"
roleName="contributor"
subscriptionId="648b0f22-f94f-4296-8c83-54f5d751b1e6"
environment="Prod"
servicePrincipalName="Azure-ARM-${environment}-${projectName}"
az ad sp create-for-rbac --name $servicePrincipalName --role $roleName --scopes /subscriptions/$subscriptionId --json-auth

## credentials

{
  "clientId": "59593b6d-5cc3-4da2-8c3f-11de9ea4e9c5",
  "clientSecret": "KC.8Q~KMTZMt65L~53uAbU_leqoh95Rr.ACYKdi9",
  "subscriptionId": "648b0f22-f94f-4296-8c83-54f5d751b1e6",
  "tenantId": "a2799098-ec71-4199-a883-6274017f5282",
  "activeDirectoryEndpointUrl": "https://login.microsoftonline.com",
  "resourceManagerEndpointUrl": "https://management.azure.com/",
  "activeDirectoryGraphResourceId": "https://graph.windows.net/",
  "sqlManagementEndpointUrl": "https://management.core.windows.net:8443/",
  "galleryEndpointUrl": "https://gallery.azure.com/",
  "managementEndpointUrl": "https://management.core.windows.net/"
}