---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConditionalAccessPolicy();



$conditions = new ConditionalAccessConditionSet();
$requestRequestBody->setConditions($conditions);


$signInRiskLevelsArray = [];
'high',$signInRiskLevelsArray []= $signInRiskLevels1;
'medium',$signInRiskLevelsArray []= $signInRiskLevels2;
'low',$signInRiskLevelsArray []= $signInRiskLevels3;
$conditions->setSignInRiskLevels($signInRiskLevelsArray);

$result =  $graphClient->identity()->conditionalAccess()->policiesById('conditionalAccessPolicy-id')->patch($requestRequestBody);


```