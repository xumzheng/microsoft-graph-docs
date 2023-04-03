---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessReviewHistoryDefinition();
requestBody.setDisplayName('Last quarter\'s group reviews April 2021');

requestBody.setDecisions([requestBody.setAccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('approve'));
requestBody.setAccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('deny'));
requestBody.setAccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('dontknow'));
requestBody.setAccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('notreviewed'));
requestBody.setAccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('notnotified'));
]);

requestBody.setReviewHistoryPeriodStartDateTime(DateTime('2021-01-01T00:00:00Z'));

requestBody.setReviewHistoryPeriodEndDateTime(DateTime('2021-04-30T23:59:59Z'));

scopesAccessReviewScope1 = AccessReviewScope();
scopesAccessReviewScope1.set@odatatype('#microsoft.graph.accessReviewQueryScope');

additionalData = [
'queryType' => 'MicrosoftGraph', 
'query' => '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'accessPackageAssignments\')', 
'queryRoot' => 	null,
];
scopesAccessReviewScope1.setAdditionalData(additionalData);



scopesArray []= scopesAccessReviewScope1;
scopesAccessReviewScope2 = AccessReviewScope();
scopesAccessReviewScope2.set@odatatype('#microsoft.graph.accessReviewQueryScope');

additionalData = [
'queryType' => 'MicrosoftGraph', 
'query' => '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'/groups\')', 
'queryRoot' => 	null,
];
scopesAccessReviewScope2.setAdditionalData(additionalData);



scopesArray []= scopesAccessReviewScope2;
requestBody.setScopes(scopesArray);




result = awaitclient.identityGovernance().accessReviews().historyDefinitions().post(requestBody);


```