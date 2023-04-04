---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = InstantiatePostRequestBody();
request_body.setDisplayName('Azure AD SAML Toolkit');



result = await client.applicationTemplatesById('applicationTemplate-id').instantiate().post(request_body);


```