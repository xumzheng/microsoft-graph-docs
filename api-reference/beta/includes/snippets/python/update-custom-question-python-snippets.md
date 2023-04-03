---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = MeetingRegistrationQuestion();
requestBody.setAnswerInputType(AnswerInputType('radiobutton'));

requestBody.setAnswerOptions(['Software Engineer', 'Software Development Manager', 'Product Manager', 'Data scientist', 'Other', ]);



result = awaitclient.me().onlineMeetingsById('onlineMeeting-id').registration().customQuestionsById('meetingRegistrationQuestion-id').patch(requestBody);


```