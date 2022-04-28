---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Chat();
requestBody.chatType = ChatType.OneOnOne;
const conversationmember = new ConversationMember();
conversationmember.roles = [
						"owner"
					]
conversationmember.additionalData = {
					 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
					 "user@odata.bind" : "https://graph.microsoft.com/beta/users('jacob@contoso.com')"
				 }
const conversationmember1 = new ConversationMember();
conversationmember1.roles = [
						"owner"
					]
conversationmember1.additionalData = {
					 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
					 "user@odata.bind" : "https://graph.microsoft.com/beta/users('alex@contoso.com')"
				 }
requestBody.members = [
			conversationmember,
			conversationmember1
		]
const result = async () => {
	await graphServiceClient.chats.post(requestBody);
}


```