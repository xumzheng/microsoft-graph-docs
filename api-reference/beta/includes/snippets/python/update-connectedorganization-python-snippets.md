---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ConnectedOrganization();
requestBody.setDisplayName('Connected organization new name');

requestBody.setDescription('Connected organization new description');

requestBody.setState(ConnectedOrganizationState('configured'));



requestResult = graphServiceClient.identityGovernance().entitlementManagement().connectedOrganizationsById('connectedOrganization-id').patch(requestBody);


```