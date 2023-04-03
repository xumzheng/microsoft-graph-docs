---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = InstantiatePostRequestBody();
requestBody.setDisplayName('Azure AD SAML Toolkit');



result = await client.applicationTemplatesById('applicationTemplate-id').instantiate().post(requestBody);


```