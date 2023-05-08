---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PrintJob = {
	displayName : "testjob",
	configuration : {
		feedOrientation : PrinterFeedOrientation.LongEdgeFirst,
		pageRanges : [
			{
				start : 1,
				end : 1,
			},
		],
		quality : PrintQuality.Medium,
		dpi : 600,
		orientation : PrintOrientation.Landscape,
		copies : 1,
		duplexMode : PrintDuplexMode.OneSided,
		colorMode : PrintColorMode.BlackAndWhite,
		inputBin : "by-pass-tray",
		outputBin : "output-tray",
		mediaSize : "A4",
		margin : {
			top : 0,
			bottom : 0,
			left : 0,
			right : 0,
		},
		mediaType : "stationery",
		finishings : null,
		pagesPerSheet : 1,
		multipageLayout : PrintMultipageLayout.ClockwiseFromBottomLeft,
		collate : false,
		scaling : PrintScaling.ShrinkToFit,
		fitPdfToPage : false,
	},
};

const result = async () => {
	await graphServiceClient.print.sharesById("printerShare-id").jobs.post(requestBody);
}


```