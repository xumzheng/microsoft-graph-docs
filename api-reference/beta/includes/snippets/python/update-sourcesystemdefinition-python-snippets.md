---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SourceSystemDefinition()
request_body.setVendor('LMS Vendor')



result = await client.external_industryData_sourceSystemsby_id('sourceSystemDefinition-id').patch(request_body)


```