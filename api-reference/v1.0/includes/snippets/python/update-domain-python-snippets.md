---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Domain();
requestBody.setIsDefault(true);

requestBody.setSupportedServices(['Email', 'OfficeCommunicationsOnline', ]);



result = awaitclient.domainsById('domain-id').patch(requestBody);


```