---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = InsightsSettings();
requestBody.setIsEnabledInOrganization(true);

requestBody.setDisabledForGroup('edbfe4fb-ec70-4300-928f-dbb2ae86c981');



result = await client.organizationById('organization-id').settings().peopleInsights().patch(requestBody);


```