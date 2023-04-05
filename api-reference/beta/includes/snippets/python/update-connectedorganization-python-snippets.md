---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConnectedOrganization()
request_body.setDisplayName('Connected organization new name')

request_body.setDescription('Connected organization new description')

request_body.setState(ConnectedOrganizationState('configured'))



result = await client.identityGovernance.entitlementManagement.connectedOrganizationsById('connectedOrganization-id').patch(request_body)


```