---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Content_type()
request_body.name = 'updatedCt'

document_set = Document_set()
document_set.should_prefix_name_to_file = True

allowed_content_types_content_type_info1 = Content_type_info()
allowed_content_types_content_type_info1.id = '0x0101'

allowed_content_types_content_type_info1.name = 'Document'


allowedContentTypesArray []= allowedContentTypesContentTypeInfo1;
document_set.allowedcontenttypes(allowedContentTypesArray)


default_contents_document_set_content1 = Document_set_content()
default_contents_document_set_content1.file_name = 'a.txt'

default_contents_document_set_content1content_type = Content_type_info()
default_contents_document_set_content1content_type.id = '0x0101'


default_contents_document_set_content1.content_type = default_contents_document_set_content1content_type

defaultContentsArray []= defaultContentsDocumentSetContent1;
default_contents_document_set_content2 = Document_set_content()
default_contents_document_set_content2.file_name = 'b.txt'

default_contents_document_set_content2content_type = Content_type_info()
default_contents_document_set_content2content_type.id = '0x0101'


default_contents_document_set_content2.content_type = default_contents_document_set_content2content_type

defaultContentsArray []= defaultContentsDocumentSetContent2;
document_set.defaultcontents(defaultContentsArray)


shared_columns_column_definition1 = Column_definition()
shared_columns_column_definition1.name = 'Description'

shared_columns_column_definition1.id = 'cbb92da4-fd46-4c7d-af6c-3128c2a5576e'


sharedColumnsArray []= sharedColumnsColumnDefinition1;
shared_columns_column_definition2 = Column_definition()
shared_columns_column_definition2.name = 'Address'

shared_columns_column_definition2.id = 'fc2e188e-ba91-48c9-9dd3-16431afddd50'


sharedColumnsArray []= sharedColumnsColumnDefinition2;
document_set.sharedcolumns(sharedColumnsArray)


welcome_page_columns_column_definition1 = Column_definition()
welcome_page_columns_column_definition1.name = 'Address'

welcome_page_columns_column_definition1.id = 'fc2e188e-ba91-48c9-9dd3-16431afddd50'


welcomePageColumnsArray []= welcomePageColumnsColumnDefinition1;
document_set.welcomepagecolumns(welcomePageColumnsArray)



request_body.document_set = document_set



result = await client.sites.by_site_id('site-id').content_types.by_content_type_id('contentType-id').patch(request_body = request_body)


```