---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReplyPostRequestBody();
$post = new Post();
$postBody = new ItemBody();
$postBody.setContentType(new BodyType('text'));

$postBody.setContent('Which quarter does that file cover? See my attachment.');


$post.setBody($postBody);
$attachmentsAttachment1 = new Attachment();
$attachmentsAttachment1.set@odatatype('#microsoft.graph.fileAttachment');

$attachmentsAttachment1.setName('Another file as attachment');

$additionalData = [
'contentBytes' => 'VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu', 
];
$attachmentsAttachment1.setAdditionalData($additionalData);



$attachmentsArray []= $attachmentsAttachment1;
$post.setAttachments($attachmentsArray);



$requestBody.setPost($post);


$graphServiceClient.groupsById('group-id').threadsById('conversationThread-id').reply().post($requestBody);


```