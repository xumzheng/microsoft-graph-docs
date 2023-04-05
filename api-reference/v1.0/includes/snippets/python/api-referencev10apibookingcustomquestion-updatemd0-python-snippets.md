---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingCustomQuestion()
request_body.set@odatatype('#microsoft.graph.bookingCustomQuestion')

request_body.setDisplayName('What is your age?')

request_body.setAnswerInputType(AnswerInputType('text'))

request_body.setAnswerOptions([])



result = await client.solutions.bookingBusinessesby_id('bookingBusiness-id').customQuestionsby_id('bookingCustomQuestion-id').patch(request_body)


```