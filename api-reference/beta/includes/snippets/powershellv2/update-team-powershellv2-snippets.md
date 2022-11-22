---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	IsMembershipLimitedToOwners = $true
	MemberSettings = @{
		AllowCreateUpdateChannels = $true
	}
	MessagingSettings = @{
		AllowUserEditMessages = $true
		AllowUserDeleteMessages = $true
	}
	FunSettings = @{
		AllowGiphy = $true
		GiphyContentRating = "strict"
	}
	DiscoverySettings = @{
		ShowInTeamsSearchAndSuggestions = $true
	}
}

Update-MgBetaTeam -TeamId $teamId -BodyParameter $params

```