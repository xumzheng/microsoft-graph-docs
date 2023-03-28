---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ConnectorGroup();
$requestBody.setName('name-value');

$requestBody.setRegion(new ConnectorGroupRegion('region-value'));



$requestResult = $graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').connectorGroupsById('connectorGroup-id').patch($requestBody);


```