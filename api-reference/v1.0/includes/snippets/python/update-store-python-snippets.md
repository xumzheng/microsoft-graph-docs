---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Store();
requestBody.setDefaultLanguageTag('en-US');



result = awaitclient.sitesById('site-id').termStore().patch(requestBody);


```