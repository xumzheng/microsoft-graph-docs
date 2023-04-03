---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = $refDeleteRequestBody();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1.0/policies/appManagementPolicies/{id}', 
];
requestBody.setAdditionalData(additionalData);




await client.applicationsById('application-id').appManagementPolicies().ref().delete(requestBody);


```