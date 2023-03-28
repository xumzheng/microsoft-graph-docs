---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReferenceCreate();
$requestBody->set@odataid('https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}');



$graphServiceClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->connectorsById('connector-id')->memberOf()->ref()->post($requestBody);


```