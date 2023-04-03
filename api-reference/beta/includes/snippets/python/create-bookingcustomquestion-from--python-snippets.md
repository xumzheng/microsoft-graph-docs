---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CustomQuestion();
additionalData = [
'@odata.type' => '#microsoft.graph.bookingCustomQuestion', 
'displayName' => 'What is your age?', 
'answerInputType' => 'text', 
'answerOptions' => [],
];
requestBody.setAdditionalData(additionalData);




awaitclient.bookingBusinessesById('bookingBusiness-id').customQuestionsById('bookingCustomQuestion-id').post(requestBody);


```