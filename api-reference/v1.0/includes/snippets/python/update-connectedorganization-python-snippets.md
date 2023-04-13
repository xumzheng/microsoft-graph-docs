---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConnectedOrganization()
request_body.displayName = 'Connected organization new name'

request_body.description = 'Connected organization new description'

request_body.State(ConnectedOrganizationState('configured'))




result = await client.identityGovernance.entitlementManagement.connectedOrganizations_by_id('connectedOrganization-id').patch(request_body = request_body)


```