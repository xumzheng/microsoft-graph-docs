---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OnPremisesAgentGroup();


$requestRequestBody->setDisplayName('Group New Name');
$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->agentGroupsById('onPremisesAgentGroup-id')->patch($requestRequestBody);


```