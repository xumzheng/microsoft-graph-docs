---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = IdentityUserFlowAttribute();
requestBody.setDescription('Your new hobby');



result = await client.identity().userFlowAttributesById('identityUserFlowAttribute-id').patch(requestBody);


```