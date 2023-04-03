---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Domain();
requestBody.setId('contoso.com');



requestResult = graphServiceClient.domains().post(requestBody);


```