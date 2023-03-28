---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new InstantiatePostRequestBody();
$requestBody.setDisplayName('Azure AD SAML Toolkit');



$requestResult = $graphServiceClient.applicationTemplatesById('applicationTemplate-id').instantiate().post($requestBody);


```