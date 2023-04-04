---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.setSource(TeamworkActivityTopicSource('entityurl'))

topic.setValue('https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7')


request_body.setTopic($topic)
request_body.setActivityType('pendingFinanceApprovalRequests')

previewText = ItemBody()
previewText.setContent('Internal spending team has a pending finance approval requests')


request_body.setPreviewText($previewText)
recipient = TeamworkNotificationRecipient()
recipient.set@odatatype('microsoft.graph.channelMembersNotificationRecipient')

additionalData = [
'teamId' => 'e8bece96-d393-4b9b-b8da-69cedef1a7e7', 
'channelId' => '19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2', 
];
recipient.setAdditionalData(additionalData)



request_body.setRecipient($recipient)
templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.setName('pendingRequestCount')

templateParametersKeyValuePair1.setValue('5')


templateParametersArray []= templateParametersKeyValuePair1;
request_body.setTemplateParameters(templateParametersArray)




await client.teamsById('team-id').sendActivityNotification.post(request_body)


```