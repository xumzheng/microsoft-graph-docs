---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = WebAccount();
request_body.setDescription('My Github contributions!');

request_body.setUserId('innocenty.popov');

service = ServiceInformation();
service.setName('GitHub');

service.setWebUrl('https://github.com');


request_body.setService($service);


result = await client.me().profile().webAccounts().post(request_body);


```