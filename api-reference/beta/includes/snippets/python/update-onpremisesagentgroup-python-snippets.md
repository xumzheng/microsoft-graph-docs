---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OnPremisesAgentGroup();
$requestBody->setDisplayName('Group New Name');



$requestResult = $graphServiceClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->agentGroupsById('onPremisesAgentGroup-id')->patch($requestBody);


```