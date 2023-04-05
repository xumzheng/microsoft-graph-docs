---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Custodian()
request_body.setEmail('AdeleV@contoso.com')

request_body.setApplyHoldToSources(true)



result = await client.compliance.ediscovery.casesby_id('case-id').custodians.post(request_body)


```