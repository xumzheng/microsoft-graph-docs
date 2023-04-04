---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.setSource(TeamworkActivityTopicSource('text'))

topic.setValue('Deployment Approvals Channel')

topic.setWebUrl('https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000')


request_body.setTopic($topic)
request_body.setActivityType('approvalRequired')

previewText = ItemBody()
previewText.setContent('New deployment requires your approval')


request_body.setPreviewText($previewText)
recipient = TeamworkNotificationRecipient()
recipient.set@odatatype('microsoft.graph.aadUserNotificationRecipient')

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipient.setAdditionalData(additionalData)



request_body.setRecipient($recipient)
templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.setName('deploymentId')

templateParametersKeyValuePair1.setValue('6788662')


templateParametersArray []= templateParametersKeyValuePair1;
request_body.setTemplateParameters(templateParametersArray)




await client.teamsById('team-id').sendActivityNotification.post(request_body)


```