---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Item()
additionalData = [
'acl' => acl1 = ()
		acl1.type = 'everyone'

		acl1.value = '67a141d8-cf4e-4528-ba07-bed21bfacd2d'

		acl1.accessType = 'grant'


aclArray []= acl1;
request_body.acl(aclArray)


];
request_body.additionaldata(additionalData)




request_configuration = ExternalItemRequestBuilderPatchRequestConfiguration(
)


await client.external.connections_by_id('externalConnection-id').items_by_id('externalItem-id').patch(request_body = request_body)


```