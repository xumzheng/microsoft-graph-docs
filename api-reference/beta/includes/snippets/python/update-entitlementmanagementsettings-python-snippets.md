---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EntitlementManagementSettings()
request_body.setExternalUserLifecycleAction('None')



result = await client.identityGovernance.entitlementManagement.settings.patch(request_body)


```