---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Acronym();
requestBody.setDescription('A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.');



result = await client.search().acronymsById('acronym-id').patch(requestBody);


```