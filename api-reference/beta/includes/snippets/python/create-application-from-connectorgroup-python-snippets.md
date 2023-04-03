---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ReferenceUpdate();
requestBody.set@odataid('https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}');



graphServiceClient.applicationsById('application-id').connectorGroup().ref().put(requestBody);


```