---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContentType()
request_body.name = 'updatedCt'

documentSet = DocumentSet()
documentSet.shouldPrefixNameToFile = true

allowedContentTypesContentTypeInfo1 = ContentTypeInfo()
allowedContentTypesContentTypeInfo1.id = '0x0101'

allowedContentTypesContentTypeInfo1.name = 'Document'


allowedContentTypesArray []= allowedContentTypesContentTypeInfo1;
documentSet.allowedcontenttypes(allowedContentTypesArray)


defaultContentsDocumentSetContent1 = DocumentSetContent()
defaultContentsDocumentSetContent1.fileName = 'a.txt'

defaultContentsDocumentSetContent1ContentType = ContentTypeInfo()
defaultContentsDocumentSetContent1ContentType.id = '0x0101'


defaultContentsDocumentSetContent1.contentType = defaultContentsDocumentSetContent1ContentType

defaultContentsArray []= defaultContentsDocumentSetContent1;
defaultContentsDocumentSetContent2 = DocumentSetContent()
defaultContentsDocumentSetContent2.fileName = 'b.txt'

defaultContentsDocumentSetContent2ContentType = ContentTypeInfo()
defaultContentsDocumentSetContent2ContentType.id = '0x0101'


defaultContentsDocumentSetContent2.contentType = defaultContentsDocumentSetContent2ContentType

defaultContentsArray []= defaultContentsDocumentSetContent2;
documentSet.defaultcontents(defaultContentsArray)


sharedColumnsColumnDefinition1 = ColumnDefinition()
sharedColumnsColumnDefinition1.name = 'Description'

sharedColumnsColumnDefinition1.id = 'cbb92da4-fd46-4c7d-af6c-3128c2a5576e'


sharedColumnsArray []= sharedColumnsColumnDefinition1;
sharedColumnsColumnDefinition2 = ColumnDefinition()
sharedColumnsColumnDefinition2.name = 'Address'

sharedColumnsColumnDefinition2.id = 'fc2e188e-ba91-48c9-9dd3-16431afddd50'


sharedColumnsArray []= sharedColumnsColumnDefinition2;
documentSet.sharedcolumns(sharedColumnsArray)


welcomePageColumnsColumnDefinition1 = ColumnDefinition()
welcomePageColumnsColumnDefinition1.name = 'Address'

welcomePageColumnsColumnDefinition1.id = 'fc2e188e-ba91-48c9-9dd3-16431afddd50'


welcomePageColumnsArray []= welcomePageColumnsColumnDefinition1;
documentSet.welcomepagecolumns(welcomePageColumnsArray)



request_body.documentSet = documentSet


request_configuration = ContentTypeRequestBuilderPatchRequestConfiguration(
)


result = await client.sites_by_id('site-id').contentTypes_by_id('contentType-id').patch(request_body = request_body)


```