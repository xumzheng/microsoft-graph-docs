---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = BookingCustomQuestion();
requestBody.set@odatatype('#microsoft.graph.bookingCustomQuestion');

requestBody.setDisplayName('What is your age?');

requestBody.setAnswerInputType(AnswerInputType('text'));

requestBody.setAnswerOptions([]);



result = awaitclient.bookingBusinessesById('bookingBusiness-id').customQuestionsById('bookingCustomQuestion-id').patch(requestBody);


```