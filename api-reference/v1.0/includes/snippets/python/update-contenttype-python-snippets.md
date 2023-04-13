---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContentType()
request_body.name = 'updatedCt'

document_set = DocumentSet()
documentSet.should_prefix_name_to_file = True

allowed_content_types_content_type_info1 = ContentTypeInfo()
allowedContentTypesContentTypeInfo1.id = '0x0101'

allowedContentTypesContentTypeInfo1.name = 'Document'


allowedContentTypesArray []= allowedContentTypesContentTypeInfo1;
documentSet.allowedcontenttypes(allowedContentTypesArray)


default_contents_document_set_content1 = DocumentSetContent()
defaultContentsDocumentSetContent1.fileName = 'a.txt'

default_contents_document_set_content1_content_type = ContentTypeInfo()
defaultContentsDocumentSetContent1ContentType.id = '0x0101'


defaultContentsDocumentSetContent1.content_type = defaultContentsDocumentSetContent1ContentType

defaultContentsArray []= defaultContentsDocumentSetContent1;
default_contents_document_set_content2 = DocumentSetContent()
defaultContentsDocumentSetContent2.fileName = 'b.txt'

default_contents_document_set_content2_content_type = ContentTypeInfo()
defaultContentsDocumentSetContent2ContentType.id = '0x0101'


defaultContentsDocumentSetContent2.content_type = defaultContentsDocumentSetContent2ContentType

defaultContentsArray []= defaultContentsDocumentSetContent2;
documentSet.defaultcontents(defaultContentsArray)


shared_columns_column_definition1 = ColumnDefinition()
sharedColumnsColumnDefinition1.name = 'Description'

sharedColumnsColumnDefinition1.id = 'cbb92da4-fd46-4c7d-af6c-3128c2a5576e'


sharedColumnsArray []= sharedColumnsColumnDefinition1;
shared_columns_column_definition2 = ColumnDefinition()
sharedColumnsColumnDefinition2.name = 'Address'

sharedColumnsColumnDefinition2.id = 'fc2e188e-ba91-48c9-9dd3-16431afddd50'


sharedColumnsArray []= sharedColumnsColumnDefinition2;
documentSet.sharedcolumns(sharedColumnsArray)


welcome_page_columns_column_definition1 = ColumnDefinition()
welcomePageColumnsColumnDefinition1.name = 'Address'

welcomePageColumnsColumnDefinition1.id = 'fc2e188e-ba91-48c9-9dd3-16431afddd50'


welcomePageColumnsArray []= welcomePageColumnsColumnDefinition1;
documentSet.welcomepagecolumns(welcomePageColumnsArray)



request_body.document_set = documentSet



result = await client.sites_by_id('site-id').contentTypes_by_id('contentType-id').patch(request_body = request_body)


```