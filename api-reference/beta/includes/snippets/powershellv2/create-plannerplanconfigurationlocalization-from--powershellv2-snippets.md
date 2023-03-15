---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Bookings

$params = @{
	"@odata.type" = "#microsoft.graph.plannerPlanConfigurationLocalization"
	LanguageTag = "en-us"
	PlanTitle = "Order Tracking"
	Buckets = @(
		@{
			"@odata.type" = "microsoft.graph.plannerPlanConfigurationBucketLocalization"
			ExternalBucketId = "deliveryBucket"
			Name = "Deliveries"
		}
		@{
			"@odata.type" = "microsoft.graph.plannerPlanConfigurationBucketLocalization"
			ExternalBucketId = "storePickupBucket"
			Name = "Pickup"
		}
		@{
			"@odata.type" = "microsoft.graph.plannerPlanConfigurationBucketLocalization"
			ExternalBucketId = "specialOrdersBucket"
			Name = "Special Orders"
		}
		@{
			"@odata.type" = "microsoft.graph.plannerPlanConfigurationBucketLocalization"
			ExternalBucketId = "returnProcessingBucket"
			Name = "Customer Returns"
		}
	)
}

New-MgBetaBusinessScenarioPlannerPlanConfigurationLocalization -BusinessScenarioId $businessScenarioId -BodyParameter $params

```