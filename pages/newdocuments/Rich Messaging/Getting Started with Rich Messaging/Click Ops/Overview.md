---
pagename: Overview
redirect_from:
  - rich-messaging-click-ops.html
Keywords:
sitesection: Documents
categoryname: "Rich Messaging"
documentname: Getting Started
subfoldername: Click Operations
order: 80
permalink: getting-started-with-rich-messaging-click-operations-overview.html
indicator: both
---

On-click operations can result from two object types:

| Property Name | Description | Type | Required | Size Limit |
| :--- | :--- | :--- | :--- | :--- |
| Actions | List of actions to execute (Navigate/Link/publish text) | action | N | 4 actions per element |
| Metadata | list of UMS predefined objects to send back to the agent |  | N |  |


### Example

```json
"click": {
	"metadata": [
		{
			"type": "ExternalId",
			"id": "someID"
		}
	],
	"actions": [
		{
			"type": "publishText",
			"text": "Show Plan"
		}
	]
}
```
