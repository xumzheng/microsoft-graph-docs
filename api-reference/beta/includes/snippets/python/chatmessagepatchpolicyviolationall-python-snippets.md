---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ChatMessage();
policyViolation = ChatMessagePolicyViolation();
policyViolationPolicyTip = ChatMessagePolicyViolationPolicyTip();
policyViolationPolicyTip.setGeneralText('This item has been blocked by the administrator.');

policyViolationPolicyTip.setComplianceUrl('https://contoso.com/dlp-policy-page');

policyViolationPolicyTip.setMatchedConditionDescriptions(['Credit Card Number', ]);


policyViolation.setPolicyTip($policyViolationPolicyTip);
policyViolation.setVerdictDetails(ChatMessagePolicyViolationVerdictDetailsTypes('allowoverridewithoutjustification,allowfalsepositiveoverride'));

policyViolation.setDlpAction(ChatMessagePolicyViolationDlpActionTypes('blockaccess'));


requestBody.setPolicyViolation($policyViolation);


result = await client.teamsById('team-id').channelsById('channel-id').messagesById('chatMessage-id').patch(requestBody);


```