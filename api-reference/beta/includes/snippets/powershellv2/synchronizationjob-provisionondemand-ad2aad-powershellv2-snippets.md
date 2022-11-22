---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	Parameters = @(
		@{
			RuleId = "6c409270-f78a-4bc6-af23-7cf3ab6482fe"
			Subjects = @(
				@{
					ObjectId = "CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com"
					ObjectTypeName = "user"
				}
			)
		}
	)
}

New-MgBetaServicePrincipalSynchronizationJobOnDemand -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId -BodyParameter $params

```