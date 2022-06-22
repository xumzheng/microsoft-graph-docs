---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Call();


$requestRequestBody->setCallbackUri('https://bot.contoso.com/callback');
$requestedModalitiesArray = [];
'audio',$requestedModalitiesArray []= $requestedModalities1;
$requestRequestBody->setRequestedModalities($requestedModalitiesArray);

$mediaConfig = new MediaConfig();
$requestRequestBody->setMediaConfig($mediaConfig);


$mediaConfigAdditionalData = [
	"@odata.type" => '#microsoft.graph.serviceHostedMediaConfig',
	"preFetchMedia" =>  [
	],
];
$mediaConfig->setAdditionalData($mediaConfigAdditionalData);


$chatInfo = new ChatInfo();
$requestRequestBody->setChatInfo($chatInfo);


$chatInfo->setThreadId('19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2');
$chatInfo->setMessageId('0');
$chatInfoAdditionalData = [
"@odata.type" => '#microsoft.graph.chatInfo',
];
$chatInfo->setAdditionalData($chatInfoAdditionalData);


$meetingInfo = new MeetingInfo();
$requestRequestBody->setMeetingInfo($meetingInfo);


$meetingInfo->setAllowConversationWithoutHost(True);
$meetingInfoAdditionalData = [
"@odata.type" => '#microsoft.graph.organizerMeetingInfo',
];
$meetingInfo->setAdditionalData($meetingInfoAdditionalData);

$requestRequestBody->setTenantId('86dc81db-c112-4228-9222-63f3esaa1edb');
$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.call',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->communications()->calls()->post($requestRequestBody);


```