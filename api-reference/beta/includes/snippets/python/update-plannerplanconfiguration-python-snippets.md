---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PlannerPlanConfiguration();
requestBody.set@odatatype('#microsoft.graph.plannerPlanConfiguration');

requestBody.setDefaultLanguage('en-us');

bucketsPlannerPlanConfigurationBucketDefinition1 = PlannerPlanConfigurationBucketDefinition();
bucketsPlannerPlanConfigurationBucketDefinition1.setExternalBucketId('deliveryBucket');


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition1;
bucketsPlannerPlanConfigurationBucketDefinition2 = PlannerPlanConfigurationBucketDefinition();
bucketsPlannerPlanConfigurationBucketDefinition2.setExternalBucketId('storePickupBucket');


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition2;
bucketsPlannerPlanConfigurationBucketDefinition3 = PlannerPlanConfigurationBucketDefinition();
bucketsPlannerPlanConfigurationBucketDefinition3.setExternalBucketId('specialOrdersBucket');


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition3;
bucketsPlannerPlanConfigurationBucketDefinition4 = PlannerPlanConfigurationBucketDefinition();
bucketsPlannerPlanConfigurationBucketDefinition4.setExternalBucketId('returnProcessingBucket');


bucketsArray []= bucketsPlannerPlanConfigurationBucketDefinition4;
requestBody.setBuckets(bucketsArray);




result = awaitclient.solutions().businessScenariosById('businessScenario-id').planner().planConfiguration().patch(requestBody);


```