---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingCustomQuestion()
request_body.@odatatype = '#microsoft.graph.bookingCustomQuestion'

request_body.displayName = 'What is your age?'

request_body.AnswerInputType(AnswerInputType('text'))

request_body.AnswerOptions([])




result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').customQuestions.post(request_body = request_body)


```