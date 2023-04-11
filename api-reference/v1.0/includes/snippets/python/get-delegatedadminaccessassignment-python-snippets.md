---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = DelegatedAdminAccessAssignmentRequestBuilderGetRequestConfiguration(
)


result = await client.tenantRelationships.delegatedAdminRelationships_by_id('delegatedAdminRelationship-id').accessAssignments_by_id('delegatedAdminAccessAssignment-id').get()


```