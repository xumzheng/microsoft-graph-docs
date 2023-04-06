---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryCase()
request_body.setDisplayName('CONTOSO LITIGATION-005')

request_body.setDescription('Project Bazooka')

request_body.setExternalId('324516')


request_config = EdiscoveryCasesRequestBuilderPostRequestConfiguration(
request_config = EdiscoveryCasesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.security.cases.ediscoveryCases.post(request_body, headers=)


```