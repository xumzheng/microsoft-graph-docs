---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BrandingDeleteRequestBody()
additionalData = [
'id' => '0', 
];
request_body.additionaldata(additionalData)





await client.organization_by_id('organization-id').branding.delete(request_body = request_body)


```