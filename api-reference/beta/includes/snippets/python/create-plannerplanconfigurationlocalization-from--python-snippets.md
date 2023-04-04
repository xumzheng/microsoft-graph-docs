---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = PlannerPlanConfigurationLocalization();
request_body.set@odatatype('#microsoft.graph.plannerPlanConfigurationLocalization');

request_body.setLanguageTag('en-us');

request_body.setPlanTitle('Order Tracking');

bucketsPlannerPlanConfigurationBucketLocalization1 = PlannerPlanConfigurationBucketLocalization();
bucketsPlannerPlanConfigurationBucketLocalization1.set@odatatype('microsoft.graph.plannerPlanConfigurationBucketLocalization');

bucketsPlannerPlanConfigurationBucketLocalization1.setExternalBucketId('deliveryBucket');

bucketsPlannerPlanConfigurationBucketLocalization1.setName('Deliveries');


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization1;
bucketsPlannerPlanConfigurationBucketLocalization2 = PlannerPlanConfigurationBucketLocalization();
bucketsPlannerPlanConfigurationBucketLocalization2.set@odatatype('microsoft.graph.plannerPlanConfigurationBucketLocalization');

bucketsPlannerPlanConfigurationBucketLocalization2.setExternalBucketId('storePickupBucket');

bucketsPlannerPlanConfigurationBucketLocalization2.setName('Pickup');


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization2;
bucketsPlannerPlanConfigurationBucketLocalization3 = PlannerPlanConfigurationBucketLocalization();
bucketsPlannerPlanConfigurationBucketLocalization3.set@odatatype('microsoft.graph.plannerPlanConfigurationBucketLocalization');

bucketsPlannerPlanConfigurationBucketLocalization3.setExternalBucketId('specialOrdersBucket');

bucketsPlannerPlanConfigurationBucketLocalization3.setName('Special Orders');


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization3;
bucketsPlannerPlanConfigurationBucketLocalization4 = PlannerPlanConfigurationBucketLocalization();
bucketsPlannerPlanConfigurationBucketLocalization4.set@odatatype('microsoft.graph.plannerPlanConfigurationBucketLocalization');

bucketsPlannerPlanConfigurationBucketLocalization4.setExternalBucketId('returnProcessingBucket');

bucketsPlannerPlanConfigurationBucketLocalization4.setName('Customer Returns');


bucketsArray []= bucketsPlannerPlanConfigurationBucketLocalization4;
request_body.setBuckets(bucketsArray);




result = await client.solutions.businessScenariosById('businessScenario-id').planner.planConfiguration.localizations.post(request_body);


```