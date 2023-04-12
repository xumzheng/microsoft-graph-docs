---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.Source(TeamworkActivityTopicSource('entityurl'))

topic.value = 'https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}'


request_body.topic = topic
request_body.activityType = 'reservationUpdated'

previewText = ItemBody()
previewText.content = 'You have moved up the queue'


request_body.previewText = previewText
recipient = TeamworkNotificationRecipient()
recipient.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => 'jacob@contoso.com', 
];
recipient.additionaldata(additionalData)



request_body.recipient = recipient
templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.name = 'reservationId'

templateParametersKeyValuePair1.value = 'TREEE433'


templateParametersArray []= templateParametersKeyValuePair1;
templateParametersKeyValuePair2 = KeyValuePair()
templateParametersKeyValuePair2.name = 'currentSlot'

templateParametersKeyValuePair2.value = '23'


templateParametersArray []= templateParametersKeyValuePair2;
request_body.templateparameters(templateParametersArray)





await client.teams_by_id('team-id').sendActivityNotification.post(request_body = request_body)


```