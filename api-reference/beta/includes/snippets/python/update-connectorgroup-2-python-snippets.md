---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ConnectorGroup();
requestBody.setName('name-value');

requestBody.setRegion(ConnectorGroupRegion('region-value'));



result = await client.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').connectorGroupsById('connectorGroup-id').patch(requestBody);


```