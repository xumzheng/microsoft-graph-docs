---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MeetingRegistrationQuestion()
request_body.setAnswerInputType(AnswerInputType('radiobutton'))

request_body.setAnswerOptions(['Software Engineer', 'Software Development Manager', 'Product Manager', 'Data scientist', 'Other', ])



result = await client.me.onlineMeetingsby_id('onlineMeeting-id').registration.customQuestionsby_id('meetingRegistrationQuestion-id').patch(request_body)


```