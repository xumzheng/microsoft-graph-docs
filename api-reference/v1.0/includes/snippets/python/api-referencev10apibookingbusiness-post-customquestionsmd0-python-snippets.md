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


request_config = CustomQuestionsRequestBuilderPostRequestConfiguration(
request_config = CustomQuestionsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').customQuestions.post(request_body, headers=)


```