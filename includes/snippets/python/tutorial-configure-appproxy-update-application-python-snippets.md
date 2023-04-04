---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Application();
request_body.setIdentifierUris(['https://contosoiwaapp-contoso.msappproxy.net', ]);

web = WebApplication();
web.setRedirectUris(['https://contosoiwaapp-contoso.msappproxy.net', ]);

web.setHomePageUrl('https://contosoiwaapp-contoso.msappproxy.net');


request_body.setWeb($web);


result = await client.applicationsById('application-id').patch(request_body);


```