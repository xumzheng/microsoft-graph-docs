---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CustomQuestion();
$additionalData = [
'@odata.type' => '#microsoft.graph.bookingCustomQuestion', 
'displayName' => 'What is your age?', 
'answerInputType' => 'text', 
'answerOptions' => [],
];
$requestBody->setAdditionalData($additionalData);




$graphServiceClient->bookingBusinessesById('bookingBusiness-id')->customQuestionsById('bookingCustomQuestion-id')->post($requestBody);


```