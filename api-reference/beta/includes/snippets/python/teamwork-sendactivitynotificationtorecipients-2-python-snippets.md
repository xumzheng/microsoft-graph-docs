---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationToRecipientsPostRequestBody()
topic = TeamworkActivityTopic()
topic.Source(TeamworkActivityTopicSource('text'))

topic.value = 'Deployment Approvals Channel'

topic.webUrl = 'https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000'


request_body.topic = topic
request_body.activityType = 'deploymentApprovalRequired'

previewText = ItemBody()
previewText.content = 'New deployment requires your approval'


request_body.previewText = previewText
templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.name = 'deploymentId'

templateParametersKeyValuePair1.value = '6788662'


templateParametersArray []= templateParametersKeyValuePair1;
request_body.templateparameters(templateParametersArray)


recipientsTeamworkNotificationRecipient1 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient1.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipientsTeamworkNotificationRecipient1.additionaldata(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient1;
recipientsTeamworkNotificationRecipient2 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient2.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => 'ab88234e-0874-477c-9638-d144296ed04f', 
];
recipientsTeamworkNotificationRecipient2.additionaldata(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient2;
recipientsTeamworkNotificationRecipient3 = TeamworkNotificationRecipient()
recipientsTeamworkNotificationRecipient3.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => '01c64f53-69aa-42c7-9b7f-9f75195d6bfc', 
];
recipientsTeamworkNotificationRecipient3.additionaldata(additionalData)



recipientsArray []= recipientsTeamworkNotificationRecipient3;
request_body.recipients(recipientsArray)




request_configuration = SendActivityNotificationToRecipientsRequestBuilderPostRequestConfiguration(
)


await client.teamwork.sendActivityNotificationToRecipients.post(request_body = request_body)


```