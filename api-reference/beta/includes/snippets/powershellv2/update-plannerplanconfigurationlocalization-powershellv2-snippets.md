---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Bookings

$params = @{
	"@odata.type" = "#microsoft.graph.plannerPlanConfigurationLocalization"
	PlanTitle = "Order Tracking"
	Buckets = @(
		@{
			ExternalBucketId = "deliveryBucket"
			Name = "Deliveries"
		}
		@{
			ExternalBucketId = "storePickupBucket"
			Name = "Pickup"
		}
		@{
			ExternalBucketId = "specialOrdersBucket"
			Name = "Special Orders"
		}
		@{
			ExternalBucketId = "returnProcessingBucket"
			Name = "Customer Returns"
		}
	)
}

Update-MgBetaBusinessScenarioPlannerPlanConfigurationLocalization -BusinessScenarioId $businessScenarioId -PlannerPlanConfigurationLocalizationId $plannerPlanConfigurationLocalizationId -BodyParameter $params

```