---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryCustodian()
request_body.setEmail('AdeleV@contoso.com')



result = await client.security_cases_ediscoveryCasesby_id('ediscoveryCase-id')_custodians.post(request_body)


```