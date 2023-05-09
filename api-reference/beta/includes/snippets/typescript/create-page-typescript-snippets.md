---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SitePage = {
	name : "test.aspx",
	title : "test",
	pageLayout : PageLayoutType.Article,
	showComments : true,
	showRecommendedPages : false,
	titleArea : {
		enableGradientEffect : true,
		imageWebUrl : "/_LAYOUTS/IMAGES/VISUALTEMPLATETITLEIMAGE.JPG",
		layout : TitleAreaLayoutType.ColorBlock,
		showAuthor : true,
		showPublishedDate : false,
		showTextBlockAboveTitle : false,
		textAboveTitle : "TEXT ABOVE TITLE",
		textAlignment : TitleAreaTextAlignmentType.Left,
		additionalData : {
			imageSourceType : 2,
			"title" : "sample1",
		},
	},
	canvasLayout : {
		horizontalSections : [
			{
				layout : HorizontalSectionLayoutType.OneThirdRightColumn,
				id : "1",
				emphasis : SectionEmphasisType.None,
				columns : [
					{
						id : "1",
						width : 8,
						webparts : [
							{
								id : "6f9230af-2a98-4952-b205-9ede4f9ef548",
								additionalData : {
									"innerHtml" : "<p><b>Hello!</b></p>",
								},
							},
						],
					},
					{
						id : "2",
						width : 4,
						webparts : [
							{
								id : "73d07dde-3474-4545-badb-f28ba239e0e1",
								additionalData : {
									"webPartType" : "d1d91016-032f-456d-98a4-721247c305e8",
									data : {
										dataVersion : "1.9",
										description : "Show an image on your page",
										title : "Image",
										properties : {
											imageSourceType : 2,
											altText : "",
											overlayText : "",
											siteid : "0264cabe-6b92-450a-b162-b0c3d54fe5e8",
											webid : "f3989670-cd37-4514-8ccb-0f7c2cbe5314",
											listid : "bdb41041-eb06-474e-ac29-87093386bb14",
											uniqueid : "d9f94b40-78ba-48d0-a39f-3cb23c2fe7eb",
											imgWidth : 4288,
											imgHeight : 2848,
											fixAspectRatio : false,
											captionText : "",
											alignment : "Center",
										},
										serverProcessedContent : {
											imageSources : [
												{
													key : "imageSource",
													value : "/_LAYOUTS/IMAGES/VISUALTEMPLATEIMAGE1.JPG",
												},
											],
											customMetadata : [
												{
													key : "imageSource",
													value : {
														siteid : "0264cabe-6b92-450a-b162-b0c3d54fe5e8",
														webid : "f3989670-cd37-4514-8ccb-0f7c2cbe5314",
														listid : "bdb41041-eb06-474e-ac29-87093386bb14",
														uniqueid : "d9f94b40-78ba-48d0-a39f-3cb23c2fe7eb",
														width : "4288",
														height : "2848",
													},
												},
											],
										},
									},
								},
							},
						],
					},
				],
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").pages.post(requestBody);
}


```