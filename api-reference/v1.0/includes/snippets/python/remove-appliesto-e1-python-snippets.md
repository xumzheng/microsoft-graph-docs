---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = $refDeleteRequestBody()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1.0/policies/appManagementPolicies/{id}', 
];
request_body.additionaldata(additionalData)





await client.applications_by_id('application-id').appManagementPolicies.ref.delete(request_body = request_body)


```