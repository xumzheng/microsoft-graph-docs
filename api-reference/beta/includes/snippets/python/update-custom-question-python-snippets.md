---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MeetingRegistrationQuestion()
request_body.setAnswerInputType(AnswerInputType('radiobutton'))

request_body.setAnswerOptions(['Software Engineer', 'Software Development Manager', 'Product Manager', 'Data scientist', 'Other', ])



result = await client.me.onlineMeetingsById('onlineMeeting-id').registration.customQuestionsById('meetingRegistrationQuestion-id').patch(request_body)


```