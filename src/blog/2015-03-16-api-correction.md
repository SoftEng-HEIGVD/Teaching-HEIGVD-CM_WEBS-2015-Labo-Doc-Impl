---
title: API Correction
date: 2015-03-16
author: Laurent
public: true
---

The response format for an `issue` was wrong pretty much in each API path around `/issues`.

The documentation described that the format contains the `owner` or `assignee` name under this format:

```json
...
{
	"firstname": "Henri",
	"lastname": "Dupont"
}
...
```

In fact, the real format is:

```json
...
{
	"name": "Henri Dupont"
}
...
```

The same error was also present for the `author` of a `comment` present in the `issue` responses.

Enjoy!