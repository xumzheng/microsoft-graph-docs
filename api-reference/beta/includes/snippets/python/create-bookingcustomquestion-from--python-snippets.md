---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomQuestion()
additionalData = [
'@odata.type' => '#microsoft.graph.bookingCustomQuestion', 
'displayName' => 'What is your age?', 
'answerInputType' => 'text', 
'answerOptions' => [],
];
request_body.setAdditionalData(additionalData)




await client.bookingBusinesses_by_id('bookingBusiness-id').customQuestions_by_id('bookingCustomQuestion-id').post(request_body)


```