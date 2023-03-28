---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AuthoredNote();
$content = new ItemBody();
$content.setContent('Please take a look at the files tagged with follow up');

$content.setContentType(new BodyType('text'));


$requestBody.setContent($content);


$requestResult = $graphServiceClient.privacy().subjectRightsRequestsById('subjectRightsRequest-id').notes().post($requestBody);


```