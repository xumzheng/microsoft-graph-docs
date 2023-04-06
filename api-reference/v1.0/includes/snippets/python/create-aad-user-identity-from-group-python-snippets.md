---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Identity()
request_body.setId('e811976d-83df-4cbd-8b9b-5215b18aa874')

request_body.setType(IdentityType('user'))


request_config = MembersRequestBuilderPostRequestConfiguration(
request_config = MembersRequestBuilderPostRequestConfiguration(query_params=)


result = await client.external.connections_by_id('externalConnection-id').groups_by_id('externalGroup-id').members.post(request_body, headers=)


```