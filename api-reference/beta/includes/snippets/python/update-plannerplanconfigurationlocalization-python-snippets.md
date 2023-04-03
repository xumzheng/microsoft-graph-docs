---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PlannerPlanConfigurationLocalization();
requestBody.set@odatatype('#microsoft.graph.plannerPlanConfigurationLocalization');

requestBody.setPlanTitle('Order Tracking');

bucketsPlannerPlanConfigurationBucketLocalization1 = PlannerPlanConfigurationBucketLocalization();
bucketsPlannerPlanConfigurationBucketLocalization1.setExternalBucketId('deliveryBucket');

bucketsPlannerPlanConfigurationBucketLocalization1.setName('Deliveries');


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization1;
bucketsPlannerPlanConfigurationBucketLocalization2 = PlannerPlanConfigurationBucketLocalization();
bucketsPlannerPlanConfigurationBucketLocalization2.setExternalBucketId('storePickupBucket');

bucketsPlannerPlanConfigurationBucketLocalization2.setName('Pickup');


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization2;
bucketsPlannerPlanConfigurationBucketLocalization3 = PlannerPlanConfigurationBucketLocalization();
bucketsPlannerPlanConfigurationBucketLocalization3.setExternalBucketId('specialOrdersBucket');

bucketsPlannerPlanConfigurationBucketLocalization3.setName('Special Orders');


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization3;
bucketsPlannerPlanConfigurationBucketLocalization4 = PlannerPlanConfigurationBucketLocalization();
bucketsPlannerPlanConfigurationBucketLocalization4.setExternalBucketId('returnProcessingBucket');

bucketsPlannerPlanConfigurationBucketLocalization4.setName('Customer Returns');


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization4;
requestBody.setBuckets(bucketsArray);




result = awaitclient.solutions().businessScenariosById('businessScenario-id').planner().planConfiguration().localizationsById('plannerPlanConfigurationLocalization-id').patch(requestBody);


```