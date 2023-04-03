---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ConnectorGroup();
requestBody.setName('name-value');

requestBody.setRegion(ConnectorGroupRegion('region-value'));



requestResult = graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').connectorGroupsById('connectorGroup-id').patch(requestBody);


```