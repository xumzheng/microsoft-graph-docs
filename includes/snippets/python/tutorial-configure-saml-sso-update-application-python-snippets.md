---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Application();
web = WebApplication();
web.setRedirectUris(['https://signin.aws.amazon.com/saml', ]);


requestBody.setWeb($web);
requestBody.setIdentifierUris(['https://signin.aws.amazon.com/saml', ]);



result = await client.applicationsById('application-id').patch(requestBody);


```