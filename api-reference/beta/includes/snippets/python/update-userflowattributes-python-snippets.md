---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = IdentityUserFlowAttribute();
requestBody.setDescription('Your new hobby');



requestResult = graphServiceClient.identity().userFlowAttributesById('identityUserFlowAttribute-id').patch(requestBody);


```