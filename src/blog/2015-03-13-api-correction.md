---
title: API Correction
date: 2014-03-13
author: Laurent
public: true
---

An issue was reported about the `POST /issues` which does not allow to create a new issue if the user has only the role
`staff`.

In the blog post of the practical work requirements, it is specified that any use can create issues. Therefore, it is not
the case.

The fix applied relax the constraint. Now, any user can create issues.

Enjoy!