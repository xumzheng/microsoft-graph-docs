---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ConversationThread();
additionalData = [
'originalStartTimeZone' => 'originalStartTimeZone-value', 
'originalEndTimeZone' => 'originalEndTimeZone-value', 
'responseStatus' => requestBody = ResponseStatus();
		requestBody.setResponse('');

		requestBody.setTime('datetime-value');


requestBody.setResponseStatus($responseStatus);

'iCalUId' => 'iCalUId-value', 
'reminderMinutesBeforeStart' => 99,
'isReminderOn' => true,
];
requestBody.setAdditionalData(additionalData);




result = await client.groupsById('group-id').threadsById('conversationThread-id').patch(requestBody);


```