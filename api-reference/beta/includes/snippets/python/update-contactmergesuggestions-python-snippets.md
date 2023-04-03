---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ContactMergeSuggestions();
requestBody.setIsEnabled(false);



requestResult = graphServiceClient.me().settings().contactMergeSuggestions().patch(requestBody);


```