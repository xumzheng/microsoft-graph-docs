---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SitePage()
request_body.name = 'test.aspx'

request_body.title = 'test'

request_body.PageLayout(PageLayoutType('article'))

request_body.show_comments = True

request_body.show_recommended_pages = False

title_area = TitleArea()
titleArea.enable_gradient_effect = True

titleArea.imageWebUrl = '/_LAYOUTS/IMAGES/VISUALTEMPLATETITLEIMAGE.JPG'

titleArea.Layout(TitleAreaLayoutType('colorblock'))

titleArea.show_author = True

titleArea.show_published_date = False

titleArea.show_text_block_above_title = False

titleArea.textAboveTitle = 'TEXT ABOVE TITLE'

titleArea.TextAlignment(TitleAreaTextAlignmentType('left'))

additionalData = [
'imageSourceType' => 2,
'title' => 'sample1', 
];
titleArea.additionaldata(additionalData)



request_body.title_area = titleArea
canvas_layout = CanvasLayout()
horizontal_sections_horizontal_section1 = HorizontalSection()
horizontalSectionsHorizontalSection1.Layout(HorizontalSectionLayoutType('onethirdrightcolumn'))

horizontalSectionsHorizontalSection1.id = '1'

horizontalSectionsHorizontalSection1.Emphasis(SectionEmphasisType('none'))

columns_horizontal_section_column1 = HorizontalSectionColumn()
columnsHorizontalSectionColumn1.id = '1'

columnsHorizontalSectionColumn1.width = 8

webparts_web_part1 = WebPart()
webpartsWebPart1.id = '6f9230af-2a98-4952-b205-9ede4f9ef548'

additionalData = [
'innerHtml' => '<p><b>Hello!</b></p>', 
];
webpartsWebPart1.additionaldata(additionalData)



webpartsArray []= webpartsWebPart1;
columnsHorizontalSectionColumn1.webparts(webpartsArray)



columnsArray []= columnsHorizontalSectionColumn1;
columns_horizontal_section_column2 = HorizontalSectionColumn()
columnsHorizontalSectionColumn2.id = '2'

columnsHorizontalSectionColumn2.width = 4

webparts_web_part1 = WebPart()
webpartsWebPart1.id = '73d07dde-3474-4545-badb-f28ba239e0e1'

additionalData = [
'webPartType' => 'd1d91016-032f-456d-98a4-721247c305e8', 
'data' => webparts_web_part1 = Data()
	webpartsWebPart1.dataVersion = '1.9'

	webpartsWebPart1.description = 'Show an image on your page'

	webpartsWebPart1.title = 'Image'

properties = Properties()
	properties.image_source_type = 2

	properties.altText = ''

	properties.overlayText = ''

	properties.siteid = '0264cabe-6b92-450a-b162-b0c3d54fe5e8'

	properties.webid = 'f3989670-cd37-4514-8ccb-0f7c2cbe5314'

	properties.listid = 'bdb41041-eb06-474e-ac29-87093386bb14'

	properties.uniqueid = 'd9f94b40-78ba-48d0-a39f-3cb23c2fe7eb'

	properties.img_width = 4288

	properties.img_height = 2848

	properties.fix_aspect_ratio = False

	properties.captionText = ''

	properties.alignment = 'Center'


webpartsWebPart1.properties = properties
server_processed_content = ServerProcessedContent()
image_sources1 = ()
	imageSources1.key = 'imageSource'

	imageSources1.value = '/_LAYOUTS/IMAGES/VISUALTEMPLATEIMAGE1.JPG'


imageSourcesArray []= imageSources1;
serverProcessedContent.imagesources(imageSourcesArray)


custom_metadata1 = ()
customMetadata1.key = 'imageSource'

custom_metadata1_value = Value()
customMetadata1Value.siteid = '0264cabe-6b92-450a-b162-b0c3d54fe5e8'

customMetadata1Value.webid = 'f3989670-cd37-4514-8ccb-0f7c2cbe5314'

customMetadata1Value.listid = 'bdb41041-eb06-474e-ac29-87093386bb14'

customMetadata1Value.uniqueid = 'd9f94b40-78ba-48d0-a39f-3cb23c2fe7eb'

customMetadata1Value.width = '4288'

customMetadata1Value.height = '2848'


customMetadata1.value = customMetadata1Value

customMetadataArray []= customMetadata1;
serverProcessedContent.custommetadata(customMetadataArray)



webpartsWebPart1.server_processed_content = serverProcessedContent

webpartsWebPart1.data = data

];
webpartsWebPart1.additionaldata(additionalData)



webpartsArray []= webpartsWebPart1;
columnsHorizontalSectionColumn2.webparts(webpartsArray)



columnsArray []= columnsHorizontalSectionColumn2;
horizontalSectionsHorizontalSection1.columns(columnsArray)



horizontalSectionsArray []= horizontalSectionsHorizontalSection1;
canvasLayout.horizontalsections(horizontalSectionsArray)



request_body.canvas_layout = canvasLayout



result = await client.sites_by_id('site-id').pages.post(request_body = request_body)


```