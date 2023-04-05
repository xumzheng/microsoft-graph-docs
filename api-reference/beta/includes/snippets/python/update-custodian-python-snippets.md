---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Custodian()
request_body.setApplyHoldToSources(false)



result = await client.compliance.ediscovery.casesby_id('case-id').custodiansby_id('custodian-id').patch(request_body)


```