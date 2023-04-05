---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.setSource(TeamworkActivityTopicSource('entityurl'))

topic.setValue('https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}')


request_body.setTopic($topic)
request_body.setActivityType('reservationUpdated')

previewText = ItemBody()
previewText.setContent('You have moved up the queue')


request_body.setPreviewText($previewText)
recipient = TeamworkNotificationRecipient()
recipient.set@odatatype('microsoft.graph.aadUserNotificationRecipient')

additionalData = [
'userId' => 'jacob@contoso.com', 
];
recipient.setAdditionalData(additionalData)



request_body.setRecipient($recipient)
templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.setName('reservationId')

templateParametersKeyValuePair1.setValue('TREEE433')


templateParametersArray []= templateParametersKeyValuePair1;
templateParametersKeyValuePair2 = KeyValuePair()
templateParametersKeyValuePair2.setName('currentSlot')

templateParametersKeyValuePair2.setValue('23')


templateParametersArray []= templateParametersKeyValuePair2;
request_body.setTemplateParameters(templateParametersArray)




await client.teamsby_id('team-id').sendActivityNotification.post(request_body)


```