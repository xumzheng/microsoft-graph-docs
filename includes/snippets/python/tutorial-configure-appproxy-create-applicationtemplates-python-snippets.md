---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = InstantiatePostRequestBody();
requestBody.setDisplayName('Contoso IWA App');



result = awaitclient.applicationTemplatesById('applicationTemplate-id').instantiate().post(requestBody);


```