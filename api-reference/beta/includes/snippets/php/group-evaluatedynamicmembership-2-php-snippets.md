---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EvaluateDynamicMembershipPostRequestBody();


$requestRequestBody->setMemberId('319b41e8-d9e4-42f8-bdc9-741113f48b33');
$requestRequestBody->setMembershipRule('(user.displayName -startsWith "EndTestUser")');
$result =  $graphClient->groups()->evaluateDynamicMembership()->post($requestRequestBody);


```