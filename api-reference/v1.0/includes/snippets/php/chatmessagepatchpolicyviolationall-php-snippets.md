---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ChatMessage();



$policyViolation = new ChatMessagePolicyViolation();
$requestRequestBody->setPolicyViolation($policyViolation);



$policyTip = new ChatMessagePolicyViolationPolicyTip();
$policyViolation->setPolicyTip($policyTip);


$policyTip->setGeneralText('This item has been blocked by the administrator.');
$policyTip->setComplianceUrl('https://contoso.com/dlp-policy-page');
$policyTip->setMatchedConditionDescriptions( [
'Credit Card Number',],

$policyViolation->setVerdictDetails(new ChatMessagePolicyViolationVerdictDetailsTypes('AllowOverrideWithoutJustification,AllowFalsePositiveOverride'));
$policyViolation->setDlpAction(new ChatMessagePolicyViolationDlpActionTypes('BlockAccess'));

$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->messagesById('chatMessage-id')->patch($requestRequestBody);


```