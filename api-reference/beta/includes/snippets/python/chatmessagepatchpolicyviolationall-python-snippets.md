---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ChatMessage();
$policyViolation = new ChatMessagePolicyViolation();
$policyViolationPolicyTip = new ChatMessagePolicyViolationPolicyTip();
$policyViolationPolicyTip->setGeneralText('This item has been blocked by the administrator.');

$policyViolationPolicyTip->setComplianceUrl('https://contoso.com/dlp-policy-page');

$policyViolationPolicyTip->setMatchedConditionDescriptions(['Credit Card Number', ]);


$policyViolation->setPolicyTip($policyViolationPolicyTip);
$policyViolation->setVerdictDetails(new ChatMessagePolicyViolationVerdictDetailsTypes('allowoverridewithoutjustification,allowfalsepositiveoverride'));

$policyViolation->setDlpAction(new ChatMessagePolicyViolationDlpActionTypes('blockaccess'));


$requestBody->setPolicyViolation($policyViolation);


$requestResult = $graphServiceClient->teamsById('team-id')->channelsById('channel-id')->messagesById('chatMessage-id')->patch($requestBody);


```