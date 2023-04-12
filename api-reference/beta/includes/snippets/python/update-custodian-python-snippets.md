---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Custodian()
request_body.applyHoldToSources = false




result = await client.compliance.ediscovery.cases_by_id('case-id').custodians_by_id('custodian-id').patch(request_body = request_body)


```