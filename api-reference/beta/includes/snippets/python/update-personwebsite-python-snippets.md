---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PersonWebsite();
requestBody.setDescription('Lyn Damer play in the Women\'s 1st Division (Toppserien) in Norway');



result = await client.me().profile().websitesById('personWebsite-id').patch(requestBody);


```