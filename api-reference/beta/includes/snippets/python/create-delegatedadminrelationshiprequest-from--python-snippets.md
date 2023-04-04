---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = DelegatedAdminRelationshipRequest()
request_body.setAction(DelegatedAdminRelationshipRequestAction('lockforapproval'))



result = await client.tenantRelationships.delegatedAdminRelationshipsById('delegatedAdminRelationship-id').requests.post(request_body)


```