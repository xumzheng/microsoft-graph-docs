---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExternalGroup()
request_body.setId('31bea3d537902000')

request_body.setDisplayName('Contoso Marketing')

request_body.setDescription('The product marketing team')



result = await client.external.connections._by_id('externalConnection-id').groups.post(request_body)


```