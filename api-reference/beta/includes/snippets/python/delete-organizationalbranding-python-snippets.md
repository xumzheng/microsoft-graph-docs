---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = BrandingDeleteRequestBody();
additionalData = [
'id' => '0', 
];
requestBody.setAdditionalData(additionalData);




await client.organizationById('organization-id').branding().delete(requestBody);


```