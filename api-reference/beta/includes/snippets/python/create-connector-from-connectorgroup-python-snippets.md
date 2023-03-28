---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReferenceCreate();
$requestBody->set@odataid('https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}');



$graphServiceClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->connectorGroupsById('connectorGroup-id')->members()->ref()->post($requestBody);


```