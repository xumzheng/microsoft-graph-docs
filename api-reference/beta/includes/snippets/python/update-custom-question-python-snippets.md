---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MeetingRegistrationQuestion();
$requestBody.setAnswerInputType(new AnswerInputType('radiobutton'));

$requestBody.setAnswerOptions(['Software Engineer', 'Software Development Manager', 'Product Manager', 'Data scientist', 'Other', ]);



$requestResult = $graphServiceClient.me().onlineMeetingsById('onlineMeeting-id').registration().customQuestionsById('meetingRegistrationQuestion-id').patch($requestBody);


```