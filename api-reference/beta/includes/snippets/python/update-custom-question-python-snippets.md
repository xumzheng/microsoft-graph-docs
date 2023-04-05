---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MeetingRegistrationQuestion()
request_body.setAnswerInputType(AnswerInputType('radiobutton'))

request_body.setAnswerOptions(['Software Engineer', 'Software Development Manager', 'Product Manager', 'Data scientist', 'Other', ])



result = await client.me.onlineMeetings._by_id('onlineMeeting-id').registration.customQuestions._by_id('meetingRegistrationQuestion-id').patch(request_body)


```