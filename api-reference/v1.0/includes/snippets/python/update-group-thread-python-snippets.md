---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConversationThread()
additionalData = [
'originalStartTimeZone' => 'originalStartTimeZone-value', 
'originalEndTimeZone' => 'originalEndTimeZone-value', 
'responseStatus' => request_body = ResponseStatus()
		request_body.setResponse('')

		request_body.setTime('datetime-value')


request_body.setResponseStatus($responseStatus)

'iCalUId' => 'iCalUId-value', 
'reminderMinutesBeforeStart' => 99,
'isReminderOn' => true,
];
request_body.setAdditionalData(additionalData)



request_config = ConversationThreadRequestBuilderPatchRequestConfiguration(
request_config = ConversationThreadRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.groups_by_id('group-id').threads_by_id('conversationThread-id').patch(request_body, headers=)


```