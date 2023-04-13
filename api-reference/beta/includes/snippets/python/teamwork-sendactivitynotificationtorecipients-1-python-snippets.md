---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationToRecipientsPostRequestBody()
topic = TeamworkActivityTopic()
topic.Source(TeamworkActivityTopicSource('entityurl'))

topic.value = 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}'


request_body.topic = topic
request_body.activityType = 'pendingFinanceApprovalRequests'

preview_text = ItemBody()
previewText.content = 'Internal spending team has a pending finance approval requests'


request_body.preview_text = previewText
recipients_teamwork_notification_recipient1 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient1.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipientsTeamworkNotificationRecipient1.additionaldata(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient1;
recipients_teamwork_notification_recipient2 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient2.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => 'ab88234e-0874-477c-9638-d144296ed04f', 
];
recipientsTeamworkNotificationRecipient2.additionaldata(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient2;
recipients_teamwork_notification_recipient3 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient3.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => '01c64f53-69aa-42c7-9b7f-9f75195d6bfc', 
];
recipientsTeamworkNotificationRecipient3.additionaldata(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient3;
request_body.recipients(recipientsArray)


template_parameters_key_value_pair1 = KeyValuePair()
templateParametersKeyValuePair1.name = 'pendingRequestCount'

templateParametersKeyValuePair1.value = '5'


templateParametersArray []= templateParametersKeyValuePair1;
request_body.templateparameters(templateParametersArray)





await client.teamwork.sendActivityNotificationToRecipients.post(request_body = request_body)


```