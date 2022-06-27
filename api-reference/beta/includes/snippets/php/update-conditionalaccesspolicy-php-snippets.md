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
'high',$signInRiskLevelsArray []= $signInRiskLevelssignInRiskLevels1;
'medium',$signInRiskLevelsArray []= $signInRiskLevelssignInRiskLevels2;
'low',$signInRiskLevelsArray []= $signInRiskLevelssignInRiskLevels3;
$conditions->setSignInRiskLevels($signInRiskLevelsArray);

$result =  $graphClient->identity()->conditionalAccess()->policiesById('conditionalAccessPolicy-id')->patch($requestRequestBody);


```