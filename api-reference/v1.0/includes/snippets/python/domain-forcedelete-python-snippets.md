---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ForceDeletePostRequestBody();
requestBody.setDisableUserAccounts(true);



await client.domainsById('domain-id').forceDelete().post(requestBody);


```