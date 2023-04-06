---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
policyViolation = ChatMessagePolicyViolation()
policyViolationPolicyTip = ChatMessagePolicyViolationPolicyTip()
policyViolationPolicyTip.setGeneralText('This item has been blocked by the administrator.')

policyViolationPolicyTip.setComplianceUrl('https://contoso.com/dlp-policy-page')

policyViolationPolicyTip.setMatchedConditionDescriptions(['Credit Card Number', ])


policyViolation.setPolicyTip($policyViolationPolicyTip)
policyViolation.setVerdictDetails(ChatMessagePolicyViolationVerdictDetailsTypes('allowoverridewithoutjustification,allowfalsepositiveoverride'))

policyViolation.setDlpAction(ChatMessagePolicyViolationDlpActionTypes('blockaccess'))


request_body.setPolicyViolation($policyViolation)

request_config = ChatMessageRequestBuilderPatchRequestConfiguration(
request_config = ChatMessageRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages_by_id('chatMessage-id').patch(request_body, headers=)


```