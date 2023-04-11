---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
policyViolation = ChatMessagePolicyViolation()
policyViolationPolicyTip = ChatMessagePolicyViolationPolicyTip()
policyViolationPolicyTip.generalText = 'This item has been blocked by the administrator.'

policyViolationPolicyTip.complianceUrl = 'https://contoso.com/dlp-policy-page'

policyViolationPolicyTip.MatchedConditionDescriptions(['Credit Card Number', ])


policyViolation.policyTip = policyViolationPolicyTip
policyViolation.VerdictDetails(ChatMessagePolicyViolationVerdictDetailsTypes('allowoverridewithoutjustification,allowfalsepositiveoverride'))

policyViolation.DlpAction(ChatMessagePolicyViolationDlpActionTypes('blockaccess'))


request_body.policyViolation = policyViolation


request_configuration = ChatMessageRequestBuilderPatchRequestConfiguration(
)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages_by_id('chatMessage-id').patch(request_body = request_body)


```