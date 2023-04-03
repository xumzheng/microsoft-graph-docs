---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = InstantiatePostRequestBody();
requestBody.setDisplayName('AWS Contoso');



requestResult = graphServiceClient.applicationTemplatesById('applicationTemplate-id').instantiate().post(requestBody);


```