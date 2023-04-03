---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PlannerUser();
favoritePlanReferences = PlannerFavoritePlanReferenceCollection();
additionalData = [
'jd8S5gOaFk2S8aWCIAJz42QAAxtD' => favoritePlanReferences = Jd8S5gOaFk2S8aWCIAJz42QAAxtD();
		favoritePlanReferences.set@odatatype('#microsoft.graph.plannerFavoritePlanReference');

		favoritePlanReferences.setOrderHint(' !');

		favoritePlanReferences.setPlanTitle('Next Release Discussion');


favoritePlanReferences.setJd8S5gOaFk2S8aWCIAJz42QAAxtD($jd8S5gOaFk2S8aWCIAJz42QAAxtD);

'7oTB5aMIAE2rVo-1N-L7RmQAGX2q' => 		null,
];
favoritePlanReferences.setAdditionalData(additionalData);



requestBody.setFavoritePlanReferences($favoritePlanReferences);
recentPlanReferences = PlannerRecentPlanReferenceCollection();
additionalData = [
'jd8S5gOaFk2S8aWCIAJz42QAAxtD' => recentPlanReferences = Jd8S5gOaFk2S8aWCIAJz42QAAxtD();
		recentPlanReferences.set@odatatype('#microsoft.graph.plannerRecentPlanReference');

		recentPlanReferences.setLastAccessedDateTime('2018-01-02T22:49:46.155Z');

		recentPlanReferences.setPlanTitle('Next Release Discussion');


recentPlanReferences.setJd8S5gOaFk2S8aWCIAJz42QAAxtD($jd8S5gOaFk2S8aWCIAJz42QAAxtD);

];
recentPlanReferences.setAdditionalData(additionalData);



requestBody.setRecentPlanReferences($recentPlanReferences);

request_config = PlannerRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc="',
];

request_config.headers = headers;


result = awaitclient.me().planner().patch(requestBody, request_config);


```