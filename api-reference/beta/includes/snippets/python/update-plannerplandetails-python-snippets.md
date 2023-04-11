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
sharedWith.additionaldata(additionalData)



request_body.sharedWith = sharedWith
categoryDescriptions = PlannerCategoryDescriptions()
categoryDescriptions.category1 = 'Indoors'

CategoryDescriptions.category3=null


request_body.categoryDescriptions = categoryDescriptions

headers = {
		'Prefer' : "return=representation",
		'If-Match' : "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
}

)


result = await client.planner.plans_by_id('plannerPlan-id').details.patch(request_body = request_body, request_configuration = request_configuration)


```