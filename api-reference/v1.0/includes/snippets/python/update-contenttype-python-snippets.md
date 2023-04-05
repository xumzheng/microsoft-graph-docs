---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContentType()
request_body.setName('updatedCt')

documentSet = DocumentSet()
documentSet.setShouldPrefixNameToFile(true)

allowedContentTypesContentTypeInfo1 = ContentTypeInfo()
allowedContentTypesContentTypeInfo1.setId('0x0101')

allowedContentTypesContentTypeInfo1.setName('Document')


allowedContentTypesArray []= allowedContentTypesContentTypeInfo1;
documentSet.setAllowedContentTypes(allowedContentTypesArray)


defaultContentsDocumentSetContent1 = DocumentSetContent()
defaultContentsDocumentSetContent1.setFileName('a.txt')

defaultContentsDocumentSetContent1ContentType = ContentTypeInfo()
defaultContentsDocumentSetContent1ContentType.setId('0x0101')


defaultContentsDocumentSetContent1.setContentType($defaultContentsDocumentSetContent1ContentType)

defaultContentsArray []= defaultContentsDocumentSetContent1;
defaultContentsDocumentSetContent2 = DocumentSetContent()
defaultContentsDocumentSetContent2.setFileName('b.txt')

defaultContentsDocumentSetContent2ContentType = ContentTypeInfo()
defaultContentsDocumentSetContent2ContentType.setId('0x0101')


defaultContentsDocumentSetContent2.setContentType($defaultContentsDocumentSetContent2ContentType)

defaultContentsArray []= defaultContentsDocumentSetContent2;
documentSet.setDefaultContents(defaultContentsArray)


sharedColumnsColumnDefinition1 = ColumnDefinition()
sharedColumnsColumnDefinition1.setName('Description')

sharedColumnsColumnDefinition1.setId('cbb92da4-fd46-4c7d-af6c-3128c2a5576e')


sharedColumnsArray []= sharedColumnsColumnDefinition1;
sharedColumnsColumnDefinition2 = ColumnDefinition()
sharedColumnsColumnDefinition2.setName('Address')

sharedColumnsColumnDefinition2.setId('fc2e188e-ba91-48c9-9dd3-16431afddd50')


sharedColumnsArray []= sharedColumnsColumnDefinition2;
documentSet.setSharedColumns(sharedColumnsArray)


welcomePageColumnsColumnDefinition1 = ColumnDefinition()
welcomePageColumnsColumnDefinition1.setName('Address')

welcomePageColumnsColumnDefinition1.setId('fc2e188e-ba91-48c9-9dd3-16431afddd50')


welcomePageColumnsArray []= welcomePageColumnsColumnDefinition1;
documentSet.setWelcomePageColumns(welcomePageColumnsArray)



request_body.setDocumentSet($documentSet)


result = await client.sitesby_id('site-id').contentTypesby_id('contentType-id').patch(request_body)


```