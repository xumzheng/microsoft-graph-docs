---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new FavoritePostRequestBody();
$requestBody.setMessageIds(['MC172851', 'MC167983', ]);



$requestResult = $graphServiceClient.admin().serviceAnnouncement().messages().favorite().post($requestBody);


```