---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PostRequestBody();



$post = new Post();
$requestRequestBody->setPost($post);



$body = new ItemBody();
$post->setBody($body);


$body->setContentType(new BodyType(''));
$body->setContent('content-value');

$post->setReceivedDateTime(new DateTime("2016-10-19T10:37:00Z"));
$post->setHasAttachments(True);

$from = new Recipient();
$post->setFrom($from);



$emailAddress = new EmailAddress();
$from->setEmailAddress($emailAddress);


$emailAddress->setName('name-value');
$emailAddress->setAddress('address-value');



$sender = new Recipient();
$post->setSender($sender);



$emailAddress = new EmailAddress();
$sender->setEmailAddress($emailAddress);


$emailAddress->setName('name-value');
$emailAddress->setAddress('address-value');


$post->setConversationThreadId('conversationThreadId-value');
$newParticipantsArray = [];

$newParticipants1 = new Recipient();

$newParticipants1AdditionalData = [
];
$newParticipants1->setAdditionalData($newParticipants1AdditionalData);

$newParticipantsArray []= $newParticipants1;
$post->setNewParticipants($newParticipantsArray);
$post->setConversationId('conversationId-value');
$post->setCreatedDateTime(new DateTime("2016-10-19T10:37:00Z"));
$post->setLastModifiedDateTime(new DateTime("2016-10-19T10:37:00Z"));
$post->setChangeKey('changeKey-value');
$post->setCategories( [
'categories-value',],
$post->setId('id-value');

$inReplyTo = new Post();
$post->setInReplyTo($inReplyTo);



$attachmentsArray = [];

$attachments1 = new Attachment();

$attachments1->setLastModifiedDateTime(new DateTime("2016-10-19T10:37:00Z"));
$attachments1->setName('name-value');
$attachments1->setContentType('contentType-value');
$attachments1->setSize(99);
$attachments1->setIsInline(True);
$attachments1->setId('id-value');
$attachments1AdditionalData = [
"@odata.type" => '#microsoft.graph.fileAttachment',
];
$attachments1->setAdditionalData($attachments1AdditionalData);

$attachmentsArray []= $attachments1;
$post->setAttachments($attachmentsArray);

$result =  $graphClient->groupsById('group-id')->threadsById('conversationThread-id')->postsById('post-id')->reply()->post($requestRequestBody);


```