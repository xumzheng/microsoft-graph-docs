---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ConnectorGroup();
requestBody.setName('Connector Group Demo');



result = await client.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').connectorGroups().post(requestBody);


```