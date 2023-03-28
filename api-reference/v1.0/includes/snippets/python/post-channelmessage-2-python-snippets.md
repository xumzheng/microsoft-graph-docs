---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ChatMessage();
$requestBody.setCreatedDateTime(new DateTime('2019-02-04T19:58:15.511Z'));

$from = new ChatMessageFromIdentitySet();
$fromUser = new Identity();
$fromUser.setId('id-value');

$fromUser.setDisplayName('Joh Doe');

$additionalData = [
'userIdentityType' => 'aadUser', 
];
$fromUser.setAdditionalData($additionalData);



$from.setUser($fromUser);

$requestBody.setFrom($from);
$body = new ItemBody();
$body.setContentType(new BodyType('html'));

$body.setContent('Hello World');


$requestBody.setBody($body);


$requestResult = $graphServiceClient.teamsById('team-id').channelsById('channel-id').messages().post($requestBody);


```