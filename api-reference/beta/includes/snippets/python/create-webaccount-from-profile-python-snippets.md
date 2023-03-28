---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new WebAccount();
$requestBody.setDescription('My Github contributions!');

$requestBody.setUserId('innocenty.popov');

$service = new ServiceInformation();
$service.setName('GitHub');

$service.setWebUrl('https://github.com');


$requestBody.setService($service);


$requestResult = $graphServiceClient.me().profile().webAccounts().post($requestBody);


```