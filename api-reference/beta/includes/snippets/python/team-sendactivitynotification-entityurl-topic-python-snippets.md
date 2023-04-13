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

preview_text = ItemBody()
previewText.content = 'You have moved up the queue'


request_body.preview_text = previewText
recipient = TeamworkNotificationRecipient()
recipient.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipient.additionaldata(additionalData)



request_body.recipient = recipient
template_parameters_key_value_pair1 = KeyValuePair()
templateParametersKeyValuePair1.name = 'reservationId'

templateParametersKeyValuePair1.value = 'TREEE433'


templateParametersArray []= templateParametersKeyValuePair1;
template_parameters_key_value_pair2 = KeyValuePair()
templateParametersKeyValuePair2.name = 'currentSlot'

templateParametersKeyValuePair2.value = '23'


templateParametersArray []= templateParametersKeyValuePair2;
request_body.templateparameters(templateParametersArray)





await client.teams_by_id('team-id').sendActivityNotification.post(request_body = request_body)


```