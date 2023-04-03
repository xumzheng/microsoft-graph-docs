---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Application();
requestBody.setIdentifierUris(['https://contosoiwaapp-contoso.msappproxy.net', ]);

web = WebApplication();
web.setRedirectUris(['https://contosoiwaapp-contoso.msappproxy.net', ]);

web.setHomePageUrl('https://contosoiwaapp-contoso.msappproxy.net');


requestBody.setWeb($web);


requestResult = graphServiceClient.applicationsById('application-id').patch(requestBody);


```