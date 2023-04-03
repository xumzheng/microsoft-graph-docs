---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PronounsSettings();
requestBody.setIsEnabledInOrganization(true);



result = awaitclient.organizationById('organization-id').settings().pronouns().patch(requestBody);


```