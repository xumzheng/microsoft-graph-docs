---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PublishedResource();
$requestBody.setDisplayName('New provisioning');

$requestBody.setResourceName('domain1.contoso.com');



$requestResult = $graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').publishedResources().post($requestBody);


```