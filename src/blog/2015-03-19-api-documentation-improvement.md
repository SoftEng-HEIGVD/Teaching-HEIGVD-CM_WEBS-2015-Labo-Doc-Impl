---
title: API Documentation Improvement
date: 2015-03-19
author: Laurent
public: true
---

Until now, the `action` `POST` `request` description on `/api/issues/:id/actions` was not precise for the action type `assign`.

This particular `state` management of the issue requires an `assigneeId`. Therefore, there is the correct format to make an assignment action.

```
{
	"type": "assign",
	"payload": {
		"assigneeId": "54d8ae183fd30364605c81b4",
		"comment" "Wonderful additional comment that is optional"
	}
}
```

Enjoy!