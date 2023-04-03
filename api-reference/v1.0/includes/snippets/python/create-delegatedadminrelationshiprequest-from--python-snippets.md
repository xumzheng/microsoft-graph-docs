---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DelegatedAdminRelationshipRequest();
requestBody.setAction(DelegatedAdminRelationshipRequestAction('lockforapproval'));



result = await client.tenantRelationships().delegatedAdminRelationshipsById('delegatedAdminRelationship-id').requests().post(requestBody);


```