---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AppManagementPolicie();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}', 
];
requestBody.setAdditionalData(additionalData);




await client.servicePrincipalsById('servicePrincipal-id').appManagementPoliciesById('appManagementPolicy-id').post(requestBody);


```