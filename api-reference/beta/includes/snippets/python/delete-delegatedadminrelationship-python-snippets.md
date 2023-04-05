---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DelegatedAdminRelationshipRequestBuilderDeleteRequestConfiguration()

headers = [
	'If-Match' => 'W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw=="',
]

request_config.headers = headers


await client.tenantRelationships.delegatedAdminRelationshipsById('delegatedAdminRelationship-id').delete(request_config)


```