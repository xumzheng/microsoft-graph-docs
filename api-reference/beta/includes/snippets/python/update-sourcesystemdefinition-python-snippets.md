---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SourceSystemDefinition();
requestBody.setVendor('LMS Vendor');



requestResult = graphServiceClient.external().industryData().sourceSystemsById('sourceSystemDefinition-id').patch(requestBody);


```