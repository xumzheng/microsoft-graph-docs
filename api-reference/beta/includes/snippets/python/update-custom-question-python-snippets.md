---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MeetingRegistrationQuestion()
request_body.AnswerInputType(AnswerInputType('radiobutton'))

request_body.AnswerOptions(['Software Engineer', 'Software Development Manager', 'Product Manager', 'Data scientist', 'Other', ])




result = await client.me.onlineMeetings_by_id('onlineMeeting-id').registration.customQuestions_by_id('meetingRegistrationQuestion-id').patch(request_body = request_body)


```