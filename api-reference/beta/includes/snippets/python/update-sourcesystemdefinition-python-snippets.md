---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SourceSystemDefinition();
requestBody.setVendor('LMS Vendor');



result = awaitclient.external().industryData().sourceSystemsById('sourceSystemDefinition-id').patch(requestBody);


```