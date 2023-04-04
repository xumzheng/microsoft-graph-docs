---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ConnectorGroup();
request_body.setName('name-value');

request_body.setRegion(ConnectorGroupRegion('region-value'));



result = await client.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').connectorGroupsById('connectorGroup-id').patch(request_body);


```