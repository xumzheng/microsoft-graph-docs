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
		request_body.@odatatype = '#microsoft.graph.accessReviewQueryScope'

		request_body.query = '/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers'

		request_body.queryType = 'MicrosoftGraph'


request_body.scope = scope

'instanceEnumerationScope' => request_body = InstanceEnumerationScope()
		request_body.@odatatype = '#microsoft.graph.accessReviewQueryScope'

		request_body.query = '/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f'

		request_body.queryType = 'MicrosoftGraph'


request_body.instanceEnumerationScope = instanceEnumerationScope

'reviewers' => [],
'settings' => request_body = Settings()
	request_body.mailNotificationsEnabled = true

	request_body.reminderNotificationsEnabled = true

	request_body.justificationRequiredOnApproval = true

	request_body.defaultDecisionEnabled = false

	request_body.defaultDecision = 'None'

	request_body.instanceDurationInDays = 3

	request_body.autoApplyDecisionsEnabled = false

	request_body.recommendationsEnabled = true

recurrence = Recurrence()
recurrencePattern = Pattern()
	recurrencePattern.type = 'weekly'

	recurrencePattern.interval = 1


recurrence.pattern = recurrencePattern
recurrenceRange = Range()
	recurrenceRange.type = 'noEnd'

	recurrenceRange.startDate = '2020-09-15'


recurrence.range = recurrenceRange

request_body.recurrence = recurrence

request_body.settings = settings

];
request_body.additionaldata(additionalData)




request_configuration = AccessReviewScheduleDefinitionRequestBuilderPutRequestConfiguration(
)


await client.identityGovernance.accessReviews.definitions_by_id('accessReviewScheduleDefinition-id').put(request_body = request_body)


```