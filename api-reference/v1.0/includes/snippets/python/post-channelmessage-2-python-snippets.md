---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ChatMessage();
requestBody.setCreatedDateTime(DateTime('2019-02-04T19:58:15.511Z'));

from = ChatMessageFromIdentitySet();
fromUser = Identity();
fromUser.setId('id-value');

fromUser.setDisplayName('Joh Doe');

additionalData = [
'userIdentityType' => 'aadUser', 
];
fromUser.setAdditionalData(additionalData);



from.setUser($fromUser);

requestBody.setFrom($from);
body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('Hello World');


requestBody.setBody($body);


requestResult = graphServiceClient.teamsById('team-id').channelsById('channel-id').messages().post(requestBody);


```