---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SourceSystemDefinition();
requestBody.setVendor('LMS Vendor');



result = await client.external().industryData().sourceSystemsById('sourceSystemDefinition-id').patch(requestBody);


```