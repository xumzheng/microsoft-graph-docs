---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.setSource(TeamworkActivityTopicSource('entityurl'))

topic.setValue('https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}')


request_body.setTopic($topic)
request_body.setActivityType('approvalRequired')

previewText = ItemBody()
previewText.setContent('Deployment requires your approval')


request_body.setPreviewText($previewText)
recipient = TeamworkNotificationRecipient()
recipient.set@odatatype('microsoft.graph.aadUserNotificationRecipient')

additionalData = [
'userId' => 'jacob@contoso.com', 
];
recipient.setAdditionalData(additionalData)



request_body.setRecipient($recipient)
templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.setName('approvalTaskId')

templateParametersKeyValuePair1.setValue('2020AAGGTAPP')


templateParametersArray []= templateParametersKeyValuePair1;
request_body.setTemplateParameters(templateParametersArray)



request_config = SendActivityNotificationRequestBuilderPostRequestConfiguration(
request_config = SendActivityNotificationRequestBuilderPostRequestConfiguration(query_params=)


await client.chats_by_id('chat-id').sendActivityNotification.post(request_body, headers=)


```