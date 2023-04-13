---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ScopedRoleMembership()
request_body.roleId = 'roleId-value'

roleMemberInfo = Identity()
roleMemberInfo.id = 'id-value'


request_body.roleMemberInfo = roleMemberInfo



result = await client.administrativeUnits_by_id('administrativeUnit-id').scopedRoleMembers.post(request_body = request_body)


```