---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AppManagementPolicie()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1.0/policies/appManagementPolicies/{id}', 
];
request_body.setAdditionalData(additionalData)




await client.servicePrincipals_by_id('servicePrincipal-id').appManagementPolicies_by_id('appManagementPolicy-id').post(request_body)


```