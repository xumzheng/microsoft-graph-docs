---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PersonAnnotation();
$detail = new ItemBody();
$detail.setContentType(new BodyType('text'));

$detail.setContent('I am originally from Australia, but grew up in Moscow, Russia.');


$requestBody.setDetail($detail);
$requestBody.setDisplayName('About Me');



$requestResult = $graphServiceClient.me().profile().notes().post($requestBody);


```