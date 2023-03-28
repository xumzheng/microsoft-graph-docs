---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Application();
$web = new WebApplication();
$web->setRedirectUris(['https://signin.aws.amazon.com/saml', ]);


$requestBody->setWeb($web);
$requestBody->setIdentifierUris(['https://signin.aws.amazon.com/saml', ]);



$requestResult = $graphServiceClient->applicationsById('application-id')->patch($requestBody);


```