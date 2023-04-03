---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = BrandingDeleteRequestBody();
additionalData = [
'id' => '0', 
];
requestBody.setAdditionalData(additionalData);




awaitclient.organizationById('organization-id').branding().delete(requestBody);


```