---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Application();
web = WebApplication();
web.setRedirectUris(['https://signin.aws.amazon.com/saml', ]);


request_body.setWeb($web);
request_body.setIdentifierUris(['https://signin.aws.amazon.com/saml', ]);



result = await client.applicationsById('application-id').patch(request_body);


```