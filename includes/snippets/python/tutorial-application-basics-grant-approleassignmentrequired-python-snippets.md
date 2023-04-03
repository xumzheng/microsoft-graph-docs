---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ServicePrincipal();
requestBody.setAppRoleAssignmentRequired(true);



requestResult = graphServiceClient.servicePrincipalsById('servicePrincipal-id').patch(requestBody);


```