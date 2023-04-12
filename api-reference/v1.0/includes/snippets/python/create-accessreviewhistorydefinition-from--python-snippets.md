---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReviewHistoryDefinition()
request_body.displayName = 'Last quarter\'s group reviews April 2021'

request_body.Decisions([request_body.AccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('approve'))
request_body.AccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('deny'))
request_body.AccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('dontknow'))
request_body.AccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('notreviewed'))
request_body.AccessReviewHistoryDecisionFilter(AccessReviewHistoryDecisionFilter('notnotified'))
])

request_body.reviewHistoryPeriodStartDateTime = DateTime('2021-01-01T00:00:00Z')

request_body.reviewHistoryPeriodEndDateTime = DateTime('2021-04-30T23:59:59Z')

scopesAccessReviewScope1 = AccessReviewScope()
scopesAccessReviewScope1.@odatatype = '#microsoft.graph.accessReviewQueryScope'

additionalData = [
'queryType' => 'MicrosoftGraph', 
'query' => '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'accessPackageAssignments\')', 
'queryRoot' => 	null,
];
scopesAccessReviewScope1.additionaldata(additionalData)



scopesArray []= scopesAccessReviewScope1;
scopesAccessReviewScope2 = AccessReviewScope()
scopesAccessReviewScope2.@odatatype = '#microsoft.graph.accessReviewQueryScope'

additionalData = [
'queryType' => 'MicrosoftGraph', 
'query' => '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'/groups\')', 
'queryRoot' => 	null,
];
scopesAccessReviewScope2.additionaldata(additionalData)



scopesArray []= scopesAccessReviewScope2;
request_body.scopes(scopesArray)





result = await client.identityGovernance.accessReviews.historyDefinitions.post(request_body = request_body)


```