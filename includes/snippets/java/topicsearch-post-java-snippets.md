---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TopicCollectionPage topics = graphClient.search().topics()
	.buildRequest()
	.get();

```