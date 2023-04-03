---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = $refDeleteRequestBody();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}', 
];
requestBody.setAdditionalData(additionalData);




graphServiceClient.applicationsById('application-id').appManagementPolicies().ref().delete(requestBody);


```