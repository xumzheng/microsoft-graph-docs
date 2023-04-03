---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SynchronizationJob();
requestBody.setTemplateId('BoxOutDelta');



requestResult = graphServiceClient.servicePrincipalsById('servicePrincipal-id').synchronization().jobs().post(requestBody);


```