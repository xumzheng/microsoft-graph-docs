---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerPlanConfiguration()
request_body.@odatatype = '#microsoft.graph.plannerPlanConfiguration'

request_body.defaultLanguage = 'en-us'

buckets_planner_plan_configuration_bucket_definition1 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition1.externalBucketId = 'deliveryBucket'


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition1;
buckets_planner_plan_configuration_bucket_definition2 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition2.externalBucketId = 'storePickupBucket'


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition2;
buckets_planner_plan_configuration_bucket_definition3 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition3.externalBucketId = 'specialOrdersBucket'


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition3;
buckets_planner_plan_configuration_bucket_definition4 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition4.externalBucketId = 'returnProcessingBucket'


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition4;
request_body.buckets(bucketsArray)





result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.planConfiguration.patch(request_body = request_body)


```