---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = BookingCustomQuestion();
requestBody.set@odatatype('#microsoft.graph.bookingCustomQuestion');

requestBody.setDisplayName('What is your age?');

requestBody.setAnswerInputType(AnswerInputType('text'));

requestBody.setAnswerOptions([]);



requestResult = graphServiceClient.solutions().bookingBusinessesById('bookingBusiness-id').customQuestionsById('bookingCustomQuestion-id').patch(requestBody);


```