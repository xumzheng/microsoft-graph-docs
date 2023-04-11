---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerUser()
favoritePlanReferences = PlannerFavoritePlanReferenceCollection()
additionalData = [
'jd8S5gOaFk2S8aWCIAJz42QAAxtD' => favoritePlanReferences = Jd8S5gOaFk2S8aWCIAJz42QAAxtD()
		favoritePlanReferences.@odatatype = '#microsoft.graph.plannerFavoritePlanReference'

		favoritePlanReferences.orderHint = ' !'

		favoritePlanReferences.planTitle = 'Next Release Discussion'


favoritePlanReferences.jd8S5gOaFk2S8aWCIAJz42QAAxtD = jd8S5gOaFk2S8aWCIAJz42QAAxtD

'7oTB5aMIAE2rVo-1N-L7RmQAGX2q' => 		null,
];
favoritePlanReferences.additionaldata(additionalData)



request_body.favoritePlanReferences = favoritePlanReferences
recentPlanReferences = PlannerRecentPlanReferenceCollection()
additionalData = [
'jd8S5gOaFk2S8aWCIAJz42QAAxtD' => recentPlanReferences = Jd8S5gOaFk2S8aWCIAJz42QAAxtD()
		recentPlanReferences.@odatatype = '#microsoft.graph.plannerRecentPlanReference'

		recentPlanReferences.lastAccessedDateTime = '2018-01-02T22:49:46.155Z'

		recentPlanReferences.planTitle = 'Next Release Discussion'


recentPlanReferences.jd8S5gOaFk2S8aWCIAJz42QAAxtD = jd8S5gOaFk2S8aWCIAJz42QAAxtD

];
recentPlanReferences.additionaldata(additionalData)



request_body.recentPlanReferences = recentPlanReferences

headers = {
		'Prefer' : "return=representation",
		'If-Match' : "W/\"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc=\"",
}

)


result = await client.me.planner.patch(request_body = request_body, request_configuration = request_configuration)


```