---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerPlanConfigurationLocalization()
request_body.@odatatype = '#microsoft.graph.plannerPlanConfigurationLocalization'

request_body.languageTag = 'en-us'

request_body.planTitle = 'Order Tracking'

bucketsPlannerPlanConfigurationBucketLocalization1 = PlannerPlanConfigurationBucketLocalization()
bucketsPlannerPlanConfigurationBucketLocalization1.@odatatype = 'microsoft.graph.plannerPlanConfigurationBucketLocalization'

bucketsPlannerPlanConfigurationBucketLocalization1.externalBucketId = 'deliveryBucket'

bucketsPlannerPlanConfigurationBucketLocalization1.name = 'Deliveries'


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization1;
bucketsPlannerPlanConfigurationBucketLocalization2 = PlannerPlanConfigurationBucketLocalization()
bucketsPlannerPlanConfigurationBucketLocalization2.@odatatype = 'microsoft.graph.plannerPlanConfigurationBucketLocalization'

bucketsPlannerPlanConfigurationBucketLocalization2.externalBucketId = 'storePickupBucket'

bucketsPlannerPlanConfigurationBucketLocalization2.name = 'Pickup'


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization2;
bucketsPlannerPlanConfigurationBucketLocalization3 = PlannerPlanConfigurationBucketLocalization()
bucketsPlannerPlanConfigurationBucketLocalization3.@odatatype = 'microsoft.graph.plannerPlanConfigurationBucketLocalization'

bucketsPlannerPlanConfigurationBucketLocalization3.externalBucketId = 'specialOrdersBucket'

bucketsPlannerPlanConfigurationBucketLocalization3.name = 'Special Orders'


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization3;
bucketsPlannerPlanConfigurationBucketLocalization4 = PlannerPlanConfigurationBucketLocalization()
bucketsPlannerPlanConfigurationBucketLocalization4.@odatatype = 'microsoft.graph.plannerPlanConfigurationBucketLocalization'

bucketsPlannerPlanConfigurationBucketLocalization4.externalBucketId = 'returnProcessingBucket'

bucketsPlannerPlanConfigurationBucketLocalization4.name = 'Customer Returns'


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization4;
request_body.buckets(bucketsArray)





result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.planConfiguration.localizations.post(request_body = request_body)


```