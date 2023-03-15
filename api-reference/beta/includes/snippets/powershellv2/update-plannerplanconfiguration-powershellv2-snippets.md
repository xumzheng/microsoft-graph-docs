---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Bookings

$params = @{
	"@odata.type" = "#microsoft.graph.plannerPlanConfiguration"
	DefaultLanguage = "en-us"
	Buckets = @(
		@{
			ExternalBucketId = "deliveryBucket"
		}
		@{
			ExternalBucketId = "storePickupBucket"
		}
		@{
			ExternalBucketId = "specialOrdersBucket"
		}
		@{
			ExternalBucketId = "returnProcessingBucket"
		}
	)
}

Update-MgBetaBusinessScenarioPlannerPlanConfiguration -BusinessScenarioId $businessScenarioId -BodyParameter $params

```