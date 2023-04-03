---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ConnectorGroup();
requestBody.setName('Connector Group Demo');



requestResult = graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').connectorGroups().post(requestBody);


```