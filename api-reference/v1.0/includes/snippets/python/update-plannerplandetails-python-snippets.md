---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerPlanDetails()
sharedWith = PlannerUserIds()
additionalData = [
'6463a5ce-2119-4198-9f2a-628761df4a62' => true,
'd95e6152-f683-4d78-9ff5-67ad180fea4a' => false,
];
sharedWith.setAdditionalData(additionalData)



request_body.setSharedWith($sharedWith)
categoryDescriptions = PlannerCategoryDescriptions()
categoryDescriptions.setCategory1('Indoors')

CategoryDescriptions.setCategory3(null)


request_body.setCategoryDescriptions($categoryDescriptions)

request_config = DetailsRequestBuilderPatchRequestConfiguration()

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
]

request_config.headers = headers


result = await client.planner.plansById('plannerPlan-id').details.patch(request_body, request_config)


```