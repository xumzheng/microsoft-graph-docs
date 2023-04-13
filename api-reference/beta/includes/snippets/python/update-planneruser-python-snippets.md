---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerUser()
favorite_plan_references = PlannerFavoritePlanReferenceCollection()
additionalData = [
'jd8S5gOaFk2S8aWCIAJz42QAAxtD' => favorite_plan_references = Jd8S5gOaFk2S8aWCIAJz42QAAxtD()
		favoritePlanReferences.@odatatype = '#microsoft.graph.plannerFavoritePlanReference'

		favoritePlanReferences.orderHint = ' !'

		favoritePlanReferences.planTitle = 'Next Release Discussion'


favoritePlanReferences.jd8_s5g_oa_fk2_s8a_w_c_i_a_jz42_q_a_axt_d = jd8S5gOaFk2S8aWCIAJz42QAAxtD

'7oTB5aMIAE2rVo-1N-L7RmQAGX2q' => 		null,
];
favoritePlanReferences.additionaldata(additionalData)



request_body.favorite_plan_references = favoritePlanReferences
recent_plan_references = PlannerRecentPlanReferenceCollection()
additionalData = [
'jd8S5gOaFk2S8aWCIAJz42QAAxtD' => recent_plan_references = Jd8S5gOaFk2S8aWCIAJz42QAAxtD()
		recentPlanReferences.@odatatype = '#microsoft.graph.plannerRecentPlanReference'

		recentPlanReferences.lastAccessedDateTime = '2018-01-02T22:49:46.155Z'

		recentPlanReferences.planTitle = 'Next Release Discussion'


recentPlanReferences.jd8_s5g_oa_fk2_s8a_w_c_i_a_jz42_q_a_axt_d = jd8S5gOaFk2S8aWCIAJz42QAAxtD

];
recentPlanReferences.additionaldata(additionalData)



request_body.recent_plan_references = recentPlanReferences


request_configuration = PlannerRequestBuilder.PlannerRequestBuilderPatchRequestConfiguration(
headers = {
		'Prefer' : "return=representation",
		'If-Match' : "W/\"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc=\"",
}

)


result = await client.me.planner.patch(request_body = request_body, request_configuration = request_configuration)


```