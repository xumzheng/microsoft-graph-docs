---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	PolicyViolation = @{
		PolicyTip = @{
			GeneralText = "This item has been blocked by the administrator."
			ComplianceUrl = "https://contoso.com/dlp-policy-page"
			MatchedConditionDescriptions = @(
				"Credit Card Number"
			)
		}
		VerdictDetails = "AllowOverrideWithoutJustification,AllowFalsePositiveOverride"
		DlpAction = "BlockAccess"
	}
}

Update-MgBetaTeamChannelMessage -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId -BodyParameter $params

```