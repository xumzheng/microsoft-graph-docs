---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = IdentityUserFlowAttribute();
requestBody.setDescription('Your new hobby');



result = awaitclient.identity().userFlowAttributesById('identityUserFlowAttribute-id').patch(requestBody);


```