---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SourceCollection()
request_body.setDisplayName('Quarterly Financials search')



result = await client.compliance.ediscovery.casesById('case-id').sourceCollectionsById('sourceCollection-id').patch(request_body)


```