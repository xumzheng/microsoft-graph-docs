---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AppManagementPolicie()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}', 
];
request_body.setAdditionalData(additionalData)




await client.servicePrincipalsById('servicePrincipal-id').appManagementPoliciesById('appManagementPolicy-id').post(request_body)


```