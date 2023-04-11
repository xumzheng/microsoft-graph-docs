---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.Source(TeamworkActivityTopicSource('text'))

topic.value = 'Weekly Virtual Social'

topic.webUrl = 'Teams webUrl'


request_body.topic = topic
previewText = ItemBody()
previewText.content = 'It will be fun!'


request_body.previewText = previewText
request_body.activityType = 'eventCreated'

recipient = TeamworkNotificationRecipient()
recipient.@odatatype = 'microsoft.graph.channelMembersNotificationRecipient'

additionalData = [
'teamId' => '7155e3c8-175e-4311-97ef-572edc3aa3db', 
'channelId' => '19:0ea5de04de4743bcb4cd20cb99235d99@thread.tacv2', 
];
recipient.additionaldata(additionalData)



request_body.recipient = recipient


request_configuration = SendActivityNotificationRequestBuilderPostRequestConfiguration(
)


await client.teams_by_id('team-id').sendActivityNotification.post(request_body = request_body)


```