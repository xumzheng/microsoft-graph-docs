---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ContactMergeSuggestions();
requestBody.setIsEnabled(false);



result = await client.me().settings().contactMergeSuggestions().patch(requestBody);


```