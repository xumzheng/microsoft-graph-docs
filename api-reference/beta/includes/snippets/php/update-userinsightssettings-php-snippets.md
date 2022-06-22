---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UserInsightsSettings();


$requestRequestBody->setIsEnabled('false');
$result =  $graphClient->usersById('user-id')->settings()->itemInsights()->patch($requestRequestBody);


```