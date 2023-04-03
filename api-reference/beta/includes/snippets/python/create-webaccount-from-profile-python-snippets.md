---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = WebAccount();
requestBody.setDescription('My Github contributions!');

requestBody.setUserId('innocenty.popov');

service = ServiceInformation();
service.setName('GitHub');

service.setWebUrl('https://github.com');


requestBody.setService($service);


result = await client.me().profile().webAccounts().post(requestBody);


```