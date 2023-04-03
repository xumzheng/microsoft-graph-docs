---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = DelegatedAdminRelationshipRequest();
requestBody.setAction(DelegatedAdminRelationshipRequestAction('lockforapproval'));



requestResult = graphServiceClient.tenantRelationships().delegatedAdminRelationshipsById('delegatedAdminRelationship-id').requests().post(requestBody);


```