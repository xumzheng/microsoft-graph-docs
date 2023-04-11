---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.@odataid = 'https://graph.microsoft.com/beta/directoryObjects/{id}'



request_configuration = RefRequestBuilderPostRequestConfiguration(
)


await client.applications_by_id('application-id').owners.ref.post(request_body = request_body)


```