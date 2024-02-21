---

excalidraw-plugin: parsed
tags: [excalidraw]

title: GPU 锁细化相关
date created: 星期四, 二月 1日 2024, 5:08:31 下午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

==⚠ Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
core 1 ^NcHhENJR

core 2 ^wqKnUG1i

core 3 ^y0iAdxEE

core 4 ^Ah7mzel3

GPU 锁 ^0t8r54rX

cpu 运行 ^vKlgOjK1

GPU 运行 ^3dGnAktv

CPU 运行 ^SIH0aVi1

task 运行顺序 ^LTvUGlLc

需要时获取这个锁 ^PxGSjV6w

获取锁 ^Bz7SSn1N

释放锁 ^gxiyGlsd

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
			"version": 44,
			"versionNonce": 1730244807,
			"isDeleted": false,
			"id": "DFlUVEounRYzLavShQYBU",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -346.75,
			"y": -241.2421875,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 239,
			"height": 51,
			"seed": 157162872,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "NcHhENJR"
				},
				{
					"id": "Icc56KjhbbVfz4ZdVOUnV",
					"type": "arrow"
				}
			],
			"updated": 1706853337656,
			"link": null,
			"locked": false
		},
		{
			"id": "NcHhENJR",
			"type": "text",
			"x": -255.28997802734375,
			"y": -228.2421875,
			"width": 56.0799560546875,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1292908457,
			"version": 43,
			"versionNonce": 898586215,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853318690,
			"link": null,
			"locked": false,
			"text": "core 1",
			"rawText": "core 1",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "DFlUVEounRYzLavShQYBU",
			"originalText": "core 1",
			"lineHeight": 1.25
		},
		{
			"type": "rectangle",
			"version": 128,
			"versionNonce": 1444438729,
			"isDeleted": false,
			"id": "ddWDilKhJhMaulbX8YKHN",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -346.6136324344164,
			"y": -162.6340040147761,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 237.04419800481227,
			"height": 51,
			"seed": 463449479,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "wqKnUG1i"
				},
				{
					"id": "4KD_GMXr16iG5k34mEhts",
					"type": "arrow"
				}
			],
			"updated": 1706853352564,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 129,
			"versionNonce": 249264679,
			"isDeleted": false,
			"id": "wqKnUG1i",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -260.54150749206883,
			"y": -149.6340040147761,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 64.89994812011719,
			"height": 25,
			"seed": 41837735,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1706853341317,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "core 2",
			"rawText": "core 2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "ddWDilKhJhMaulbX8YKHN",
			"originalText": "core 2",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 87,
			"versionNonce": 594384199,
			"isDeleted": false,
			"id": "iSKn6Gs4VdqSYBxCFTLIX",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -347.85037010989606,
			"y": -84.08282830710147,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 239,
			"height": 51,
			"seed": 1961250281,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "y0iAdxEE"
				},
				{
					"id": "CcmFW8tyYDo1Q49m1vng_",
					"type": "arrow"
				}
			],
			"updated": 1706853395614,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 88,
			"versionNonce": 1436608839,
			"isDeleted": false,
			"id": "y0iAdxEE",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -260.4903466113609,
			"y": -71.08282830710147,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 64.27995300292969,
			"height": 25,
			"seed": 1687595209,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1706853325443,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "core 3",
			"rawText": "core 3",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "iSKn6Gs4VdqSYBxCFTLIX",
			"originalText": "core 3",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "rectangle",
			"version": 125,
			"versionNonce": 804608329,
			"isDeleted": false,
			"id": "0qrh8XJOTGDiseCUNBjll",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -343.8023985539371,
			"y": -3.3097125400031473,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 239,
			"height": 51,
			"seed": 2000201641,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Ah7mzel3"
				}
			],
			"updated": 1706853318691,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 127,
			"versionNonce": 1833129513,
			"isDeleted": false,
			"id": "Ah7mzel3",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -256.0323713932926,
			"y": 9.690287459996853,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 63.45994567871094,
			"height": 25,
			"seed": 653773449,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1706853328273,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "core 4",
			"rawText": "core 4",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "0qrh8XJOTGDiseCUNBjll",
			"originalText": "core 4",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"id": "Icc56KjhbbVfz4ZdVOUnV",
			"type": "arrow",
			"x": -102.41655779328515,
			"y": -210.19216181723533,
			"width": 149.61885263185854,
			"height": 64.3503628860827,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 385566345,
			"version": 54,
			"versionNonce": 453319881,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853645593,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					149.61885263185854,
					64.3503628860827
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "DFlUVEounRYzLavShQYBU",
				"gap": 5.333442206714835,
				"focus": -0.6260318715327615
			},
			"endBinding": {
				"elementId": "i6qe7Z-lB2J9rNh61TnYe",
				"gap": 1.9558019951876986,
				"focus": -0.012658227848101198
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "4KD_GMXr16iG5k34mEhts",
			"type": "arrow",
			"x": -104.37235978847286,
			"y": -139.82107621639267,
			"width": 144.72934764388935,
			"height": 25.34501267956675,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 60972135,
			"version": 54,
			"versionNonce": 1129922185,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853645593,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					144.72934764388935,
					25.34501267956675
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "ddWDilKhJhMaulbX8YKHN",
				"gap": 5.197074641131238,
				"focus": -0.5264732348852623
			},
			"endBinding": {
				"elementId": "i6qe7Z-lB2J9rNh61TnYe",
				"gap": 8.801108978344587,
				"focus": -0.2035238952304266
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "CcmFW8tyYDo1Q49m1vng_",
			"type": "arrow",
			"x": -107.85037010989606,
			"y": -66.67294089927204,
			"width": 146.25155597012485,
			"height": 33.9786879805752,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 140360199,
			"version": 73,
			"versionNonce": 1850182409,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853645593,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					146.25155597012485,
					-33.9786879805752
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "iSKn6Gs4VdqSYBxCFTLIX",
				"gap": 1,
				"focus": 0.37370089917486216
			},
			"endBinding": {
				"elementId": "i6qe7Z-lB2J9rNh61TnYe",
				"gap": 10.756910973532285,
				"focus": 0.08948281013725878
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "v_xnQb_BQmU9s5mWs02fr",
			"type": "arrow",
			"x": -105.35026078606671,
			"y": 17.583203740373733,
			"width": 150.5967536294524,
			"height": 106.45929506098497,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 1330925513,
			"version": 96,
			"versionNonce": 1854179657,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853645593,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					150.5967536294524,
					-106.45929506098497
				]
			],
			"lastCommittedPoint": null,
			"startBinding": null,
			"endBinding": {
				"elementId": "i6qe7Z-lB2J9rNh61TnYe",
				"gap": 3.911603990375397,
				"focus": 0.2802663438256659
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "i6qe7Z-lB2J9rNh61TnYe",
			"type": "rectangle",
			"x": 49.15809683376108,
			"y": -170.17378779764493,
			"width": 149.61885263185866,
			"height": 112.45861472329244,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 969766025,
			"version": 89,
			"versionNonce": 1299168903,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "v_xnQb_BQmU9s5mWs02fr",
					"type": "arrow"
				},
				{
					"id": "CcmFW8tyYDo1Q49m1vng_",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "0t8r54rX"
				},
				{
					"id": "Icc56KjhbbVfz4ZdVOUnV",
					"type": "arrow"
				},
				{
					"id": "4KD_GMXr16iG5k34mEhts",
					"type": "arrow"
				},
				{
					"id": "I3t0xVtemkjVL0XxjZlFD",
					"type": "arrow"
				}
			],
			"updated": 1706853563557,
			"link": null,
			"locked": false
		},
		{
			"id": "0t8r54rX",
			"type": "text",
			"x": 87.3275313894365,
			"y": -126.44448043599871,
			"width": 73.27998352050781,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 227393897,
			"version": 47,
			"versionNonce": 1698699495,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853506122,
			"link": null,
			"locked": false,
			"text": "GPU 锁",
			"rawText": "GPU 锁",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "i6qe7Z-lB2J9rNh61TnYe",
			"originalText": "GPU 锁",
			"lineHeight": 1.25
		},
		{
			"id": "NWbNxryk9R-XH4M84n17Q",
			"type": "rectangle",
			"x": 500.94835772211854,
			"y": -248.4058676051527,
			"width": 159.3978626077969,
			"height": 75.29837681472623,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 344043625,
			"version": 180,
			"versionNonce": 803001673,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "vKlgOjK1"
				}
			],
			"updated": 1706853571546,
			"link": null,
			"locked": false
		},
		{
			"id": "vKlgOjK1",
			"type": "text",
			"x": 540.0173070313881,
			"y": -223.2566791977896,
			"width": 81.25996398925781,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 156480393,
			"version": 165,
			"versionNonce": 1107641385,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853571546,
			"link": null,
			"locked": false,
			"text": "cpu 运行",
			"rawText": "cpu 运行",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "NWbNxryk9R-XH4M84n17Q",
			"originalText": "cpu 运行",
			"lineHeight": 1.25
		},
		{
			"id": "H7vmade1xKWnizBHpuNDO",
			"type": "rectangle",
			"x": 506.8157637076814,
			"y": -90.96380699254337,
			"width": 156.46415961501566,
			"height": 56.7182578604432,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 2042038663,
			"version": 294,
			"versionNonce": 2001709703,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "3dGnAktv"
				},
				{
					"id": "I3t0xVtemkjVL0XxjZlFD",
					"type": "arrow"
				}
			],
			"updated": 1706853660258,
			"link": null,
			"locked": false
		},
		{
			"id": "3dGnAktv",
			"type": "text",
			"x": 538.4078517549353,
			"y": -75.10467806232177,
			"width": 93.27998352050781,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 609754729,
			"version": 194,
			"versionNonce": 1093058983,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853660258,
			"link": null,
			"locked": false,
			"text": "GPU 运行",
			"rawText": "GPU 运行",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "H7vmade1xKWnizBHpuNDO",
			"originalText": "GPU 运行",
			"lineHeight": 1.25
		},
		{
			"id": "2cYm8-Ed9C22yBOq0tqTU",
			"type": "rectangle",
			"x": 508.7494667004632,
			"y": 52.80973865615829,
			"width": 162.33156560057853,
			"height": 66.49726783638164,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 1201969065,
			"version": 218,
			"versionNonce": 32072775,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "SIH0aVi1"
				}
			],
			"updated": 1706853650228,
			"link": null,
			"locked": false
		},
		{
			"id": "SIH0aVi1",
			"type": "text",
			"x": 544.7252623181353,
			"y": 73.55837257434911,
			"width": 90.37997436523438,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1927182183,
			"version": 212,
			"versionNonce": 1273185127,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853650228,
			"link": null,
			"locked": false,
			"text": "CPU 运行",
			"rawText": "CPU 运行",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "2cYm8-Ed9C22yBOq0tqTU",
			"originalText": "CPU 运行",
			"lineHeight": 1.25
		},
		{
			"id": "Iuwf5NTgmlAWKxLTZe0y3",
			"type": "rectangle",
			"x": 487.25774375580454,
			"y": -310.99153145115895,
			"width": 202.42550650192663,
			"height": 448.85655789557586,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 1892724009,
			"version": 205,
			"versionNonce": 827298023,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853626646,
			"link": null,
			"locked": false
		},
		{
			"id": "LTvUGlLc",
			"type": "text",
			"x": 515.616872686026,
			"y": -299.2567194800328,
			"width": 135.23995971679688,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1823512231,
			"version": 128,
			"versionNonce": 735038249,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853571547,
			"link": null,
			"locked": false,
			"text": "task 运行顺序",
			"rawText": "task 运行顺序",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "task 运行顺序",
			"lineHeight": 1.25
		},
		{
			"id": "I3t0xVtemkjVL0XxjZlFD",
			"type": "arrow",
			"x": 497.75893635591973,
			"y": -120.66539459296334,
			"width": 289.20297691436133,
			"height": 21.1321961290013,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"seed": 744328105,
			"version": 278,
			"versionNonce": 61180423,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853662658,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-289.20297691436133,
					21.1321961290013
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "hxA-QdhGyEaA_5C5wguAM",
				"focus": -0.02292562815319279,
				"gap": 10.034728349355703
			},
			"endBinding": {
				"elementId": "i6qe7Z-lB2J9rNh61TnYe",
				"focus": 0.33377057736162874,
				"gap": 9.779009975938664
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "PxGSjV6w",
			"type": "text",
			"x": 276.0311282755338,
			"y": -139.85885687223572,
			"width": 160,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 827577577,
			"version": 75,
			"versionNonce": 401396553,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853663873,
			"link": null,
			"locked": false,
			"text": "需要时获取这个锁",
			"rawText": "需要时获取这个锁",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "需要时获取这个锁",
			"lineHeight": 1.25
		},
		{
			"id": "hxA-QdhGyEaA_5C5wguAM",
			"type": "rectangle",
			"x": 507.79366470527543,
			"y": -152.5715698409557,
			"width": 151.57465462704636,
			"height": 49.8729508772862,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"seed": 1927220327,
			"version": 53,
			"versionNonce": 60800167,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "Bz7SSn1N"
				},
				{
					"id": "I3t0xVtemkjVL0XxjZlFD",
					"type": "arrow"
				}
			],
			"updated": 1706853662314,
			"link": null,
			"locked": false
		},
		{
			"id": "Bz7SSn1N",
			"type": "text",
			"x": 553.5809920187986,
			"y": -140.1350944023126,
			"width": 60,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 220693095,
			"version": 15,
			"versionNonce": 2975975,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1706853645018,
			"link": null,
			"locked": false,
			"text": "获取锁",
			"rawText": "获取锁",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "hxA-QdhGyEaA_5C5wguAM",
			"originalText": "获取锁",
			"lineHeight": 1.25
		},
		{
			"type": "rectangle",
			"version": 130,
			"versionNonce": 1567398951,
			"isDeleted": false,
			"id": "V5nKYwW6jDHxYBCRDwMJK",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 513.1279221872296,
			"y": -16.629549510589385,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 151.57465462704636,
			"height": 49.8729508772862,
			"seed": 316119847,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "gxiyGlsd"
				}
			],
			"updated": 1706853651469,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 119,
			"versionNonce": 1923049033,
			"isDeleted": false,
			"id": "gxiyGlsd",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 558.9152495007528,
			"y": -4.193074071946285,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 60,
			"height": 25,
			"seed": 1403493959,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1706853657476,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "释放锁",
			"rawText": "释放锁",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "V5nKYwW6jDHxYBCRDwMJK",
			"originalText": "释放锁",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "image",
			"version": 84,
			"versionNonce": 39670153,
			"isDeleted": true,
			"id": "cGrSOuQr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 20.314835782135276,
			"y": 116.29890989656695,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 312.5,
			"height": 500,
			"seed": 23027,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1706854021819,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "700a2df1cc3374094f4dc4fe213d0b3cc742c08a",
			"scale": [
				1,
				1
			]
		},
		{
			"text": "📍[[../slurm utilization question]]",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"id": "YiCIiS6h",
			"type": "text",
			"x": -3.5725115161355916,
			"y": 7.096542760167154,
			"width": 334.5406494140625,
			"height": 25,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"roundness": null,
			"seed": 86710,
			"version": 29,
			"versionNonce": 715169447,
			"updated": 1706854022429,
			"isDeleted": true,
			"groupIds": [],
			"boundElements": [],
			"link": "[[../slurm utilization question]]",
			"locked": false,
			"containerId": null,
			"originalText": "📍[[../slurm utilization question]]",
			"rawText": "[[../slurm utilization question]]",
			"lineHeight": 1.25
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
		"currentItemFontFamily": 1,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 547.4821669479044,
		"scrollY": 509.78193860047503,
		"zoom": {
			"value": 0.9794825200833952
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