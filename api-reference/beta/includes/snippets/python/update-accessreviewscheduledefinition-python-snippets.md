---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Definition()
additionalData = [
'id' => '60860cdd-fb4d-4054-91ba-f75e04444aa6', 
'displayName' => 'Test world UPDATED NAME!', 
'descriptionForAdmins' => 'Test world', 
'descriptionForReviewers' => 'Test world', 
'scope' => request_body = Scope()
		request_body.set@odatatype('#microsoft.graph.accessReviewQueryScope')

		request_body.setQuery('/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers')

		request_body.setQueryType('MicrosoftGraph')


request_body.setScope($scope)

'instanceEnumerationScope' => request_body = InstanceEnumerationScope()
		request_body.set@odatatype('#microsoft.graph.accessReviewQueryScope')

		request_body.setQuery('/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f')

		request_body.setQueryType('MicrosoftGraph')


request_body.setInstanceEnumerationScope($instanceEnumerationScope)

'reviewers' => [],
'settings' => request_body = Settings()
	request_body.setMailNotificationsEnabled(true)

	request_body.setReminderNotificationsEnabled(true)

	request_body.setJustificationRequiredOnApproval(true)

	request_body.setDefaultDecisionEnabled(false)

	request_body.setDefaultDecision('None')

	request_body.setInstanceDurationInDays(3)

	request_body.setAutoApplyDecisionsEnabled(false)

	request_body.setRecommendationsEnabled(true)

recurrence = Recurrence()
recurrencePattern = Pattern()
	recurrencePattern.setType('weekly')

	recurrencePattern.setInterval(1)


recurrence.setPattern($recurrencePattern)
recurrenceRange = Range()
	recurrenceRange.setType('noEnd')

	recurrenceRange.setStartDate('2020-09-15')


recurrence.setRange($recurrenceRange)

request_body.setRecurrence($recurrence)

request_body.setSettings($settings)

];
request_body.setAdditionalData(additionalData)




await client.identityGovernance.accessReviews.definitionsById('accessReviewScheduleDefinition-id').put(request_body)


```