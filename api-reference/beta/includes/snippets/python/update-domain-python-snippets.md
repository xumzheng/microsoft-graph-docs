---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Domain();
requestBody.setIsDefault(true);

requestBody.setSupportedServices(['Email', 'OfficeCommunicationsOnline', ]);



result = await client.domainsById('domain-id').patch(requestBody);


```