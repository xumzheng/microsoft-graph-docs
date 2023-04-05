---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ScopedRoleMembership()
request_body.setRoleId('roleId-value')

roleMemberInfo = Identity()
roleMemberInfo.setId('id-value')


request_body.setRoleMemberInfo($roleMemberInfo)


result = await client.administrativeUnits._by_id('administrativeUnit-id').scopedRoleMembers.post(request_body)


```