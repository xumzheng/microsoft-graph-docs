---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReviewInstanceDecisionItem();


$requestRequestBody->setDecision('Approve');
$requestRequestBody->setJustification('Kathleen still needs access to the Marketing group as she works in the Marketing organization.');
$result =  $graphClient->identityGovernance()->accessReviews()->definitionsById('accessReviewScheduleDefinition-id')->instancesById('accessReviewInstance-id')->decisionsById('accessReviewInstanceDecisionItem-id')->patch($requestRequestBody);


```