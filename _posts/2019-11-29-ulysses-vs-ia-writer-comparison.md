---
title: Ulysses vs. iA Writer Comparison - From a CJK Perspective
categories: English
tags: 写作日常
---

*(CJK stands for “Chinese, Japanese, Korean”.)*

**TLDR:**

- Both apps offer a free trial, so I encourage everyone to try them.
- If you write in CJK, iA might be better.


I have been shopping for a Markdown text editor for a while, and I like both Ulysses and iA Writer. Many articles compare the two, so I’m not going to repeat that.

This article is about writing in CJK and a tiny bug I found in Ulysses that makes me take the development team’s background into consideration.<!--more-->

The bug I found in Ulysses is super tiny:

- Test Case: type the letter ‘a’ using the MacOS Chinese input method.

![]({{ site.url}}/assets/img/ulysses_bug_line_shifting.mov.gif)

Notice the 2nd paragraph shifts for about 1px.

- Test Case: after typing the letter ‘a’, press “command + z” to undo. Surprisingly, the word selector does not disappear. So I hit ‘space’ in an attempt to select a word to remove the selector. Then for some reason, the line break is also deleted.

![]({{ site.url}}/assets/img/ulysses_bug_undo.mov.gif)

  - Expected: “undo” will undo my previous action.
  - Actual: the word selector does not disappear.

In comparison, here’s the UX in iA Writer:

![]({{ site.url}}/assets/img/ia_same.mov.gif)

I work on frontend development, and I know how difficult i18n is. Bugs like this just happen all the time. Sometimes, there is just no way to continuously test the app except for regularly using it.

For this reason, I think iA writer has and will continue to have better support in CJK. In case you don’t know yet, iA writer is developed by a Japanese company. If there’s an issue with CJK, the development team will likely catch it before the users.

If you write in CJK, this may be a factor to consider.