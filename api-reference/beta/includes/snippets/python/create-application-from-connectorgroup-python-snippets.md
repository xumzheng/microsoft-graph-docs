---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ReferenceUpdate();
requestBody.set@odataid('https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}');



await client.applicationsById('application-id').connectorGroup().ref().put(requestBody);


```