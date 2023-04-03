---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ConnectorGroup();
requestBody.setName('name-value');

requestBody.setIsDefault(false);



result = awaitclient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').connectorGroups().post(requestBody);


```