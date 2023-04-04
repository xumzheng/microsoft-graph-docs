---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessReviewHistoryDefinition()
request_body.setDisplayName('Last quarter\'s group reviews April 2021')

request_body.setDecisions([request_body.setAccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('approve'))
request_body.setAccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('deny'))
request_body.setAccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('dontknow'))
request_body.setAccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('notreviewed'))
request_body.setAccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('notnotified'))
])

request_body.setReviewHistoryPeriodStartDateTime(DateTime('2021-01-01T00:00:00Z'))

request_body.setReviewHistoryPeriodEndDateTime(DateTime('2021-04-30T23:59:59Z'))

scopesAccessReviewScope1 = AccessReviewScope()
scopesAccessReviewScope1.set@odatatype('#microsoft.graph.accessReviewQueryScope')

additionalData = [
'queryType' => 'MicrosoftGraph', 
'query' => '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'accessPackageAssignments\')', 
'queryRoot' => 	null,
];
scopesAccessReviewScope1.setAdditionalData(additionalData)



scopesArray []= scopesAccessReviewScope1;
scopesAccessReviewScope2 = AccessReviewScope()
scopesAccessReviewScope2.set@odatatype('#microsoft.graph.accessReviewQueryScope')

additionalData = [
'queryType' => 'MicrosoftGraph', 
'query' => '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'/groups\')', 
'queryRoot' => 	null,
];
scopesAccessReviewScope2.setAdditionalData(additionalData)



scopesArray []= scopesAccessReviewScope2;
request_body.setScopes(scopesArray)




result = await client.identityGovernance.accessReviews.historyDefinitions.post(request_body)


```