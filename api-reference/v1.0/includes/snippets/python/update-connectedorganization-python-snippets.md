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


request_config = ConnectedOrganizationRequestBuilderPatchRequestConfiguration(
request_config = ConnectedOrganizationRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.identityGovernance.entitlementManagement.connectedOrganizations_by_id('connectedOrganization-id').patch(request_body, headers=)


```