---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Item()
additionalData = [
'acl' => acl1 = ()
		acl1.setType('everyone')

		acl1.setValue('67a141d8-cf4e-4528-ba07-bed21bfacd2d')

		acl1.setAccessType('grant')


aclArray []= acl1;
request_body.setAcl(aclArray)


];
request_body.setAdditionalData(additionalData)




await client.external_connectionsby_id('externalConnection-id')_itemsby_id('externalItem-id').patch(request_body)


```