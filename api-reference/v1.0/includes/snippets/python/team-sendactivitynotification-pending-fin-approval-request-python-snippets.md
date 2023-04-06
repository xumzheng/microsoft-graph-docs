---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.setSource(TeamworkActivityTopicSource('entityurl'))

topic.setValue('https://graph.microsoft.com/v1.0/teams/{teamId}')


request_body.setTopic($topic)
request_body.setActivityType('pendingFinanceApprovalRequests')

previewText = ItemBody()
previewText.setContent('Internal spending team has a pending finance approval requests')


request_body.setPreviewText($previewText)
recipient = TeamworkNotificationRecipient()
recipient.set@odatatype('microsoft.graph.aadUserNotificationRecipient')

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipient.setAdditionalData(additionalData)



request_body.setRecipient($recipient)
templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.setName('pendingRequestCount')

templateParametersKeyValuePair1.setValue('5')


templateParametersArray []= templateParametersKeyValuePair1;
request_body.setTemplateParameters(templateParametersArray)



request_config = SendActivityNotificationRequestBuilderPostRequestConfiguration(
request_config = SendActivityNotificationRequestBuilderPostRequestConfiguration(query_params=)


await client.teams_by_id('team-id').sendActivityNotification.post(request_body, headers=)


```