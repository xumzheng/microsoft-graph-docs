---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EntitlementManagementSettings();
requestBody.setExternalUserLifecycleAction('None');



requestResult = graphServiceClient.identityGovernance().entitlementManagement().settings().patch(requestBody);


```