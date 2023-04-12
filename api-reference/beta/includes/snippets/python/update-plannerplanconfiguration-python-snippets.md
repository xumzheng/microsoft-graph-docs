---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerPlanConfiguration()
request_body.@odatatype = '#microsoft.graph.plannerPlanConfiguration'

request_body.defaultLanguage = 'en-us'

bucketsPlannerPlanConfigurationBucketDefinition1 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition1.externalBucketId = 'deliveryBucket'


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition1;
bucketsPlannerPlanConfigurationBucketDefinition2 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition2.externalBucketId = 'storePickupBucket'


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition2;
bucketsPlannerPlanConfigurationBucketDefinition3 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition3.externalBucketId = 'specialOrdersBucket'


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition3;
bucketsPlannerPlanConfigurationBucketDefinition4 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition4.externalBucketId = 'returnProcessingBucket'


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition4;
request_body.buckets(bucketsArray)





result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.planConfiguration.patch(request_body = request_body)


```