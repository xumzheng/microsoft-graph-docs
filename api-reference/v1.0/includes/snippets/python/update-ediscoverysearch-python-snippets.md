---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoverySearch()
request_body.setDisplayName('Teams search')



result = await client.security_cases_ediscoveryCasesby_id('ediscoveryCase-id')_searchesby_id('ediscoverySearch-id').patch(request_body)


```