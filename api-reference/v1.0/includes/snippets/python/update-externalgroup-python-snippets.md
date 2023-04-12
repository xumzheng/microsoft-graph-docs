---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExternalGroup()
request_body.displayName = 'Contoso Marketing'

request_body.description = 'The product marketing team'




result = await client.external.connections_by_id('externalConnection-id').groups_by_id('externalGroup-id').patch(request_body = request_body)


```