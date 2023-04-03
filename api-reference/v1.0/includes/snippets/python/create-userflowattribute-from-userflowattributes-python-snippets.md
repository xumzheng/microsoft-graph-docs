---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = IdentityUserFlowAttribute();
requestBody.setDisplayName('Hobby');

requestBody.setDescription('Your hobby');

requestBody.setDataType(IdentityUserFlowAttributeDataType('string'));



result = await client.identity().userFlowAttributes().post(requestBody);


```