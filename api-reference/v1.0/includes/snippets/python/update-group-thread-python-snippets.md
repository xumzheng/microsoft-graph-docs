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
		request_body.response = ''

		request_body.time = 'datetime-value'


request_body.responseStatus = responseStatus

'iCalUId' => 'iCalUId-value', 
'reminderMinutesBeforeStart' => 99,
'isReminderOn' => true,
];
request_body.additionaldata(additionalData)





result = await client.groups_by_id('group-id').threads_by_id('conversationThread-id').patch(request_body = request_body)


```