---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PronounsSettings();
requestBody.setIsEnabledInOrganization(true);



result = await client.organizationById('organization-id').settings().pronouns().patch(requestBody);


```