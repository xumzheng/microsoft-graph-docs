---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	DisplayName = "Finance"
	Members = @(
		@{
			UserId = "92f6952f-61ca-4a94-8910-508a240bc167"
		}
		@{
			UserId = "085d800c-b86b-4bfc-a857-9371ad1caf29"
		}
	)
}

New-MgBetaTeamTag -TeamId $teamId -BodyParameter $params

```