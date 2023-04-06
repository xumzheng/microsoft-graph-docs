---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerPlanConfiguration()
request_body.set@odatatype('#microsoft.graph.plannerPlanConfiguration')

request_body.setDefaultLanguage('en-us')

bucketsPlannerPlanConfigurationBucketDefinition1 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition1.setExternalBucketId('deliveryBucket')


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition1;
bucketsPlannerPlanConfigurationBucketDefinition2 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition2.setExternalBucketId('storePickupBucket')


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition2;
bucketsPlannerPlanConfigurationBucketDefinition3 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition3.setExternalBucketId('specialOrdersBucket')


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition3;
bucketsPlannerPlanConfigurationBucketDefinition4 = PlannerPlanConfigurationBucketDefinition()
bucketsPlannerPlanConfigurationBucketDefinition4.setExternalBucketId('returnProcessingBucket')


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition4;
request_body.setBuckets(bucketsArray)



request_config = PlanConfigurationRequestBuilderPatchRequestConfiguration(
request_config = PlanConfigurationRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.planConfiguration.patch(request_body, headers=)


```