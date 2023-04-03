---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CustomQuestion();
additionalData = [
'@odata.type' => '#microsoft.graph.bookingCustomQuestion', 
'displayName' => 'What is your age?', 
'answerInputType' => 'text', 
'answerOptions' => [],
];
requestBody.setAdditionalData(additionalData);




await client.bookingBusinessesById('bookingBusiness-id').customQuestionsById('bookingCustomQuestion-id').post(requestBody);


```