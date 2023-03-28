---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new BookingCustomQuestion();
$requestBody.set@odatatype('#microsoft.graph.bookingCustomQuestion');

$requestBody.setDisplayName('What is your age?');

$requestBody.setAnswerInputType(new AnswerInputType('text'));

$requestBody.setAnswerOptions([]);



$requestResult = $graphServiceClient.solutions().bookingBusinessesById('bookingBusiness-id').customQuestions().post($requestBody);


```