---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = DelegatedAdminRelationshipRequestBuilderDeleteRequestConfiguration(
headers = {
					'If-Match' : "W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"",
}

)


await client.tenantRelationships.delegatedAdminRelationships_by_id('delegatedAdminRelationship-id').delete(request_configuration = request_configuration)


```