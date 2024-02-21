---

excalidraw-plugin: parsed
tags: [excalidraw]

title: Slurm work flow
date created: 星期三, 二月 21日 2024, 11:16:53 上午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

==⚠ Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
User ^K04oy0rv

node ^DYwTZUSY

ssh connect ^ARxnFsSo

slurm partition ^J7gh9xmG

partition compute node ^owfoX2H2

compute node1 ^oYS18TwW

compute node2 ^qJxwUPcL

compute node4 ^Obn3m6uW

compute node3 ^qZGMOMmf

compute nodeN ^xqq6Gcao

compute node5 ^W7RgRHb0

Slurm Work Flow ^UScmTDS6

Job ^n6km5M8Q

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.28",
	"elements": [
		{
			"type": "rectangle",
			"version": 172,
			"versionNonce": 587551519,
			"isDeleted": false,
			"id": "VUABEGR-Jn8QanNfdgQ7H",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -330.3333333333337,
			"y": -188.2421875000009,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1058.333333333334,
			"height": 458.3333333333338,
			"seed": 1979139615,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "UScmTDS6"
				}
			],
			"updated": 1708486226409,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 60,
			"versionNonce": 2143010239,
			"isDeleted": false,
			"id": "UScmTDS6",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 62.15462239583326,
			"y": -183.2421875000009,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 273.357421875,
			"height": 41.4,
			"seed": 602065457,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486795338,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "Slurm Work Flow",
			"rawText": "Slurm Work Flow",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": "VUABEGR-Jn8QanNfdgQ7H",
			"originalText": "Slurm Work Flow",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "rectangle",
			"version": 401,
			"versionNonce": 1026108479,
			"isDeleted": false,
			"id": "iaJ-rDwrbLF-fduGHM1SZ",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -295.33333333333326,
			"y": -119.5755208333336,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#ffec99",
			"width": 205,
			"height": 91,
			"seed": 1659402527,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "K04oy0rv"
				},
				{
					"id": "DZc1RtlJcaxGSJYCs6Cks",
					"type": "arrow"
				}
			],
			"updated": 1708485953844,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 389,
			"versionNonce": 170893087,
			"isDeleted": false,
			"id": "K04oy0rv",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -230.83723958333326,
			"y": -94.7755208333336,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 76.0078125,
			"height": 41.4,
			"seed": 1137852735,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486677389,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "User",
			"rawText": "User",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "iaJ-rDwrbLF-fduGHM1SZ",
			"originalText": "User",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "arrow",
			"version": 1272,
			"versionNonce": 978171775,
			"isDeleted": false,
			"id": "DZc1RtlJcaxGSJYCs6Cks",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -88.59793522901543,
			"y": -69.55654577757755,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 229.93126856234858,
			"height": 1.6212908640287935,
			"seed": 835111071,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ARxnFsSo"
				}
			],
			"updated": 1708496378979,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "iaJ-rDwrbLF-fduGHM1SZ",
				"gap": 1.7353981043178237,
				"focus": 0.07426688876568674
			},
			"endBinding": {
				"elementId": "Qqy4_Rqbi_zAC3CD5yqAT",
				"gap": 6.000000000000114,
				"focus": -0.07442423919741864
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					96.26460189568226,
					0.9810249442443251
				],
				[
					229.93126856234858,
					-0.6402659197844685
				]
			]
		},
		{
			"type": "text",
			"version": 44,
			"versionNonce": 1707257279,
			"isDeleted": false,
			"id": "ARxnFsSo",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -67.04329427083317,
			"y": -84.67552083333322,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 149.419921875,
			"height": 32.199999999999996,
			"seed": 472888849,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486766387,
			"link": null,
			"locked": false,
			"fontSize": 28,
			"fontFamily": 2,
			"text": "ssh connect",
			"rawText": "ssh connect",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "DZc1RtlJcaxGSJYCs6Cks",
			"originalText": "ssh connect",
			"lineHeight": 1.15,
			"baseline": 25
		},
		{
			"type": "rectangle",
			"version": 271,
			"versionNonce": 60738527,
			"isDeleted": false,
			"id": "Qqy4_Rqbi_zAC3CD5yqAT",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 147.33333333333326,
			"y": -119.90885416666674,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 198,
			"height": 90,
			"seed": 1530041041,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "DYwTZUSY"
				},
				{
					"id": "DZc1RtlJcaxGSJYCs6Cks",
					"type": "arrow"
				},
				{
					"id": "5h4Ht7mraORDrv1Uv02jU",
					"type": "arrow"
				}
			],
			"updated": 1708486787782,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 172,
			"versionNonce": 1096640287,
			"isDeleted": false,
			"id": "DYwTZUSY",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 206.29036458333326,
			"y": -95.60885416666675,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 80.0859375,
			"height": 41.4,
			"seed": 210083263,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486775554,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "node",
			"rawText": "node",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Qqy4_Rqbi_zAC3CD5yqAT",
			"originalText": "node",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "rectangle",
			"version": 294,
			"versionNonce": 571908127,
			"isDeleted": false,
			"id": "no1Pf5xoyuT6YF1nd7rLg",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -300.3333333333339,
			"y": 69.42447916666674,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#a5d8ff",
			"width": 282,
			"height": 99,
			"seed": 238283601,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "J7gh9xmG"
				},
				{
					"id": "_oeQw_BA78EGToMcEiwN1",
					"type": "arrow"
				},
				{
					"id": "DZc1RtlJcaxGSJYCs6Cks",
					"type": "arrow"
				},
				{
					"id": "5h4Ht7mraORDrv1Uv02jU",
					"type": "arrow"
				}
			],
			"updated": 1708486787782,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 248,
			"versionNonce": 709708735,
			"isDeleted": false,
			"id": "J7gh9xmG",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -272.3694661458339,
			"y": 98.22447916666674,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 226.072265625,
			"height": 41.4,
			"seed": 1505341137,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486679136,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "slurm partition",
			"rawText": "slurm partition",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "no1Pf5xoyuT6YF1nd7rLg",
			"originalText": "slurm partition",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "rectangle",
			"version": 284,
			"versionNonce": 2033052767,
			"isDeleted": false,
			"id": "F6IsDOxdjoge2IE8alw4d",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 90.33333333333292,
			"y": 23.757812499999986,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#a5d8ff",
			"width": 591.6666666666665,
			"height": 209.00000000000003,
			"seed": 1952001439,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "owfoX2H2"
				},
				{
					"id": "_oeQw_BA78EGToMcEiwN1",
					"type": "arrow"
				}
			],
			"updated": 1708496378986,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 297,
			"versionNonce": 945304767,
			"isDeleted": false,
			"id": "owfoX2H2",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 243.73990885416617,
			"y": 28.757812499999986,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 284.853515625,
			"height": 32.199999999999996,
			"seed": 732867103,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708496378987,
			"link": null,
			"locked": false,
			"fontSize": 28,
			"fontFamily": 2,
			"text": "partition compute node",
			"rawText": "partition compute node",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": "F6IsDOxdjoge2IE8alw4d",
			"originalText": "partition compute node",
			"lineHeight": 1.15,
			"baseline": 25
		},
		{
			"type": "rectangle",
			"version": 192,
			"versionNonce": 2106361873,
			"isDeleted": false,
			"id": "MNz6o7DHWAyUU8dKtUDO2",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 129.66666666666617,
			"y": 75.75781249999989,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 167.33333333333326,
			"height": 56.333333333333364,
			"seed": 1032068895,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "oYS18TwW"
				}
			],
			"updated": 1708486751100,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 194,
			"versionNonce": 1673747953,
			"isDeleted": false,
			"id": "oYS18TwW",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 144.3929036458328,
			"y": 92.42447916666657,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 137.880859375,
			"height": 23,
			"seed": 1270863985,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486751100,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "compute node1",
			"rawText": "compute node1",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "MNz6o7DHWAyUU8dKtUDO2",
			"originalText": "compute node1",
			"lineHeight": 1.15,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 236,
			"versionNonce": 1818523601,
			"isDeleted": false,
			"id": "CzBqhg78t0z9F9xH4Gd87",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 128.66666666666617,
			"y": 159.92447916666674,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 170.66666666666652,
			"height": 56.33333333333325,
			"seed": 1174738417,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "qJxwUPcL"
				}
			],
			"updated": 1708486751100,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 261,
			"versionNonce": 1502041521,
			"isDeleted": false,
			"id": "qJxwUPcL",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 145.05957031249943,
			"y": 176.59114583333337,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 137.880859375,
			"height": 23,
			"seed": 229584849,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486751100,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "compute node2",
			"rawText": "compute node2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "CzBqhg78t0z9F9xH4Gd87",
			"originalText": "compute node2",
			"lineHeight": 1.15,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 211,
			"versionNonce": 1045657489,
			"isDeleted": false,
			"id": "gv4W86uDqkNUX0IU2x-uR",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 318.6666666666662,
			"y": 73.59114583333326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 154,
			"height": 58,
			"seed": 427004639,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Obn3m6uW"
				}
			],
			"updated": 1708486751100,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 215,
			"versionNonce": 1560305009,
			"isDeleted": false,
			"id": "Obn3m6uW",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 326.7262369791662,
			"y": 91.09114583333326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 137.880859375,
			"height": 23,
			"seed": 73129727,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486751100,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "compute node4",
			"rawText": "compute node4",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "gv4W86uDqkNUX0IU2x-uR",
			"originalText": "compute node4",
			"lineHeight": 1.15,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 285,
			"versionNonce": 1154844497,
			"isDeleted": false,
			"id": "OpRo9L_MUP9Fo648jgRlU",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 318.3333333333327,
			"y": 159.59114583333326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 154,
			"height": 58,
			"seed": 326303057,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "qZGMOMmf"
				}
			],
			"updated": 1708486751100,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 288,
			"versionNonce": 808088881,
			"isDeleted": false,
			"id": "qZGMOMmf",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 326.3929036458327,
			"y": 177.09114583333326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 137.880859375,
			"height": 23,
			"seed": 2007575345,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486751100,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "compute node3",
			"rawText": "compute node3",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "OpRo9L_MUP9Fo648jgRlU",
			"originalText": "compute node3",
			"lineHeight": 1.15,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 300,
			"versionNonce": 577152785,
			"isDeleted": false,
			"id": "QLn3Neo70BI33lAMcAfcu",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 506.99999999999966,
			"y": 161.59114583333326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 154,
			"height": 58,
			"seed": 421191249,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "xqq6Gcao"
				}
			],
			"updated": 1708486751100,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 311,
			"versionNonce": 1174510833,
			"isDeleted": false,
			"id": "xqq6Gcao",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 513.3994140624997,
			"y": 179.09114583333326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 141.201171875,
			"height": 23,
			"seed": 531426353,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486751100,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "compute nodeN",
			"rawText": "compute nodeN",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "QLn3Neo70BI33lAMcAfcu",
			"originalText": "compute nodeN",
			"lineHeight": 1.15,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 189,
			"versionNonce": 176346833,
			"isDeleted": false,
			"id": "eDd2v-vCKstE0wOiD2-rm",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 507.6666666666662,
			"y": 68.59114583333326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#b2f2bb",
			"width": 154,
			"height": 58,
			"seed": 405174399,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "W7RgRHb0"
				}
			],
			"updated": 1708486751100,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 193,
			"versionNonce": 42063025,
			"isDeleted": false,
			"id": "W7RgRHb0",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 515.7262369791662,
			"y": 86.09114583333326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 137.880859375,
			"height": 23,
			"seed": 585175199,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486751100,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "compute node5",
			"rawText": "compute node5",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "eDd2v-vCKstE0wOiD2-rm",
			"originalText": "compute node5",
			"lineHeight": 1.15,
			"baseline": 18
		},
		{
			"type": "freedraw",
			"version": 142,
			"versionNonce": 1943448799,
			"isDeleted": false,
			"id": "miJ7drqWDgkyHq_WFj0NX",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 549.6666666666662,
			"y": 144.7578125,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 127328017,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486756757,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 143,
			"versionNonce": 420291665,
			"isDeleted": false,
			"id": "1wQE008DxjYohccTg33ge",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 580.9999999999994,
			"y": 144.7578125,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 905776305,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486758868,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 141,
			"versionNonce": 321371103,
			"isDeleted": false,
			"id": "dg1Uz3scPc9K4zRlcZhRy",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 615.6666666666662,
			"y": 143.09114583333326,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 519216721,
			"groupIds": [
				"cgviZ2yPr2imbakkJjw9S"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486753256,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "arrow",
			"version": 860,
			"versionNonce": 1303879839,
			"isDeleted": false,
			"id": "_oeQw_BA78EGToMcEiwN1",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -14.333333333333883,
			"y": 124.85894489794939,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 93.66666666666686,
			"height": 2.113671440424312,
			"seed": 21596415,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1708496378986,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "no1Pf5xoyuT6YF1nd7rLg",
				"gap": 4.000000000000007,
				"focus": 0.049016364368156866
			},
			"endBinding": {
				"elementId": "F6IsDOxdjoge2IE8alw4d",
				"gap": 11.000000000000043,
				"focus": -0.05071943000937446
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					93.66666666666686,
					2.113671440424312
				]
			]
		},
		{
			"type": "arrow",
			"version": 57,
			"versionNonce": 1607715903,
			"isDeleted": false,
			"id": "5h4Ht7mraORDrv1Uv02jU",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 145.42149217522356,
			"y": -23.522203414465146,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 207.42149217522373,
			"height": 76.94668258113131,
			"seed": 105064849,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "n6km5M8Q"
				}
			],
			"updated": 1708496378983,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "Qqy4_Rqbi_zAC3CD5yqAT",
				"gap": 6.666666666666288,
				"focus": -0.17071245312807917
			},
			"endBinding": {
				"elementId": "no1Pf5xoyuT6YF1nd7rLg",
				"gap": 16.00000000000057,
				"focus": -0.28870933671314386
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-207.42149217522373,
					76.94668258113131
				]
			]
		},
		{
			"type": "text",
			"version": 4,
			"versionNonce": 1414580479,
			"isDeleted": false,
			"id": "n6km5M8Q",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 18.761067708333144,
			"y": -1.0088541666671382,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 45.14453125,
			"height": 32.199999999999996,
			"seed": 989320465,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1708486790602,
			"link": null,
			"locked": false,
			"fontSize": 28,
			"fontFamily": 2,
			"text": "Job",
			"rawText": "Job",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "5h4Ht7mraORDrv1Uv02jU",
			"originalText": "Job",
			"lineHeight": 1.15,
			"baseline": 25
		}
	],
	"appState": {
		"theme": "light",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#1e1e1e",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "solid",
		"currentItemStrokeWidth": 2,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 2,
		"currentItemFontSize": 36,
		"currentItemTextAlign": "center",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 376.8809523809524,
		"scrollY": 413.1305803571435,
		"zoom": {
			"value": 1.05
		},
		"currentItemRoundness": "round",
		"gridSize": null,
		"gridColor": {
			"Bold": "#C9C9C9FF",
			"Regular": "#EDEDEDFF"
		},
		"currentStrokeOptions": null,
		"previousGridSize": null,
		"frameRendering": {
			"enabled": true,
			"clip": true,
			"name": true,
			"outline": true
		}
	},
	"files": {}
}
```
%%