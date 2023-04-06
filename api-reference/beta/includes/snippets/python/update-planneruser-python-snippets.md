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
		favoritePlanReferences.set@odatatype('#microsoft.graph.plannerFavoritePlanReference')

		favoritePlanReferences.setOrderHint(' !')

		favoritePlanReferences.setPlanTitle('Next Release Discussion')


favoritePlanReferences.setJd8S5gOaFk2S8aWCIAJz42QAAxtD($jd8S5gOaFk2S8aWCIAJz42QAAxtD)

'7oTB5aMIAE2rVo-1N-L7RmQAGX2q' => 		null,
];
favoritePlanReferences.setAdditionalData(additionalData)



request_body.setFavoritePlanReferences($favoritePlanReferences)
recentPlanReferences = PlannerRecentPlanReferenceCollection()
additionalData = [
'jd8S5gOaFk2S8aWCIAJz42QAAxtD' => recentPlanReferences = Jd8S5gOaFk2S8aWCIAJz42QAAxtD()
		recentPlanReferences.set@odatatype('#microsoft.graph.plannerRecentPlanReference')

		recentPlanReferences.setLastAccessedDateTime('2018-01-02T22:49:46.155Z')

		recentPlanReferences.setPlanTitle('Next Release Discussion')


recentPlanReferences.setJd8S5gOaFk2S8aWCIAJz42QAAxtD($jd8S5gOaFk2S8aWCIAJz42QAAxtD)

];
recentPlanReferences.setAdditionalData(additionalData)



request_body.setRecentPlanReferences($recentPlanReferences)

request_configuration = PlannerRequestBuilderPatchRequestConfiguration(
request_configuration = PlannerRequestBuilderPatchRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.me.planner.patch(request_body, request_configuration)


```