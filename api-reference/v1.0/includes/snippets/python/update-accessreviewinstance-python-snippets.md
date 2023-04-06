---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReviewInstance()
scope = AccessReviewScope()
scope.set@odatatype('#microsoft.graph.principalResourceMembershipsScope')

additionalData = [
'principalScopes' => principalScopes1 = ()
		principalScopes1.set@odatatype('#microsoft.graph.accessReviewQueryScope')

		principalScopes1.setQuery('/v1.0/users')

		principalScopes1.setQueryType('MicrosoftGraph')


principalScopesArray []= principalScopes1;
principalScopes2 = ()
		principalScopes2.set@odatatype('#microsoft.graph.accessReviewQueryScope')

		principalScopes2.setQuery('/v1.0/groups')

		principalScopes2.setQueryType('MicrosoftGraph')


principalScopesArray []= principalScopes2;
scope.setPrincipalScopes(principalScopesArray)


'resourceScopes' => resourceScopes1 = ()
	resourceScopes1.set@odatatype('#microsoft.graph.accessReviewQueryScope')

	resourceScopes1.setQuery('/beta/roleManagement/directory/roleDefinitions/9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3')

	resourceScopes1.setQueryType('MicrosoftGraph')


resourceScopesArray []= resourceScopes1;
scope.setResourceScopes(resourceScopesArray)


];
scope.setAdditionalData(additionalData)



request_body.setScope($scope)
reviewersAccessReviewReviewerScope1 = AccessReviewReviewerScope()
reviewersAccessReviewReviewerScope1.setQuery('/users/1ed8ac56-4827-4733-8f80-86adc2e67db5')

reviewersAccessReviewReviewerScope1.setQueryType('MicrosoftGraph')


reviewersArray []= reviewersAccessReviewReviewerScope1;
request_body.setReviewers(reviewersArray)


fallbackReviewersAccessReviewReviewerScope1 = AccessReviewReviewerScope()
fallbackReviewersAccessReviewReviewerScope1.setQuery('/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e')

fallbackReviewersAccessReviewReviewerScope1.setQueryType('MicrosoftGraph')


fallbackReviewersArray []= fallbackReviewersAccessReviewReviewerScope1;
fallbackReviewersAccessReviewReviewerScope2 = AccessReviewReviewerScope()
fallbackReviewersAccessReviewReviewerScope2.setQuery('/users/1ed8ac56-4827-4733-8f80-86adc2e67db5')

fallbackReviewersAccessReviewReviewerScope2.setQueryType('MicrosoftGraph')


fallbackReviewersArray []= fallbackReviewersAccessReviewReviewerScope2;
request_body.setFallbackReviewers(fallbackReviewersArray)




result = await client.identityGovernance.accessReviews.definitions_by_id('accessReviewScheduleDefinition-id').instances_by_id('accessReviewInstance-id').patch(request_body)


```