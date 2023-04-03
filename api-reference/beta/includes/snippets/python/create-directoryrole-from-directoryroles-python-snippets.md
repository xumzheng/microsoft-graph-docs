---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DirectoryRole();
requestBody.setRoleTemplateId('fe930be7-5e62-47db-91af-98c3a49a38b1');



result = await client.directoryRoles().post(requestBody);


```