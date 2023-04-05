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

'uid' => 'iCalUId-value', 
'reminderMinutesBeforeStart' => 99,
'isReminderOn' => true,
];
request_body.setAdditionalData(additionalData)




result = await client.groupsby_id('group-id').threadsby_id('conversationThread-id').patch(request_body)


```