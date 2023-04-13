---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ScopedRoleMembership()
request_body.roleId = 'roleId-value'

role_member_info = Identity()
roleMemberInfo.id = 'id-value'


request_body.role_member_info = roleMemberInfo



result = await client.directory.administrativeUnits_by_id('administrativeUnit-id').scopedRoleMembers.post(request_body = request_body)


```