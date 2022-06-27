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

$post->setReceivedDateTime(new DateTime("datetime-value"));
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

$newParticipantsnewParticipants1 = new Recipient();

$newParticipantsnewParticipants1AdditionalData = [
];
$newParticipantsnewParticipants1->setAdditionalData($newParticipantsnewParticipants1AdditionalData);

$newParticipantsArray []= $newParticipantsnewParticipants1;
$post->setNewParticipants($newParticipantsArray);
$post->setConversationId('conversationId-value');
$post->setCreatedDateTime(new DateTime("datetime-value"));
$post->setLastModifiedDateTime(new DateTime("datetime-value"));
$post->setChangeKey('changeKey-value');
$post->setCategories(['categories-value',]);
$post->setId('id-value');

$inReplyTo = new Post();
$post->setInReplyTo($inReplyTo);



$attachmentsArray = [];

$attachmentsattachments1 = new Attachment();

$attachmentsattachments1->setLastModifiedDateTime(new DateTime("datetime-value"));
$attachmentsattachments1->setName('name-value');
$attachmentsattachments1->setContentType('contentType-value');
$attachmentsattachments1->setSize(99);
$attachmentsattachments1->setIsInline(True);
$attachmentsattachments1->setId('id-value');
$attachmentsattachments1AdditionalData = [
"@odata.type" => '#microsoft.graph.fileAttachment',
];
$attachmentsattachments1->setAdditionalData($attachmentsattachments1AdditionalData);

$attachmentsArray []= $attachmentsattachments1;
$post->setAttachments($attachmentsArray);

$result =  $graphClient->groupsById('group-id')->threadsById('conversationThread-id')->postsById('post-id')->reply()->post($requestRequestBody);


```