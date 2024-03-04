---
layout: post
title: a post with table of contents
date: 2023-03-20 11:59:00-0400
description: an example of a blog post with table of contents
tags: formatting toc
categories: sample-posts
giscus_comments: true
related_posts: false
toc:
  beginning: true
---

This post shows how to add a table of contents in the beginning of the post.

第一步 open loop
我们现在的问题并不是说场景representation啊，encoding部分不对，而是我们只学了conditional distribution p(y|x). 不管是连续还是离散的x/y, 其实问题的关键都不是单独的x 或者单独的y, 而是要把y|x 看成一个整体。视频生成任务是的，

不是说我们去学一个准确的data distribution 就行了，关键问题是：我们要学的data distribution 是什么？
p(y|x) = p(x,y)| p(x) = p(y) p (x|y) | p(x)
--> p(y|x) ~ p(y) p (x|y) (trajectory distribution * occ distribution)

p(s_t1, s_t, a_t) / p(s_t, a_t) = p(s_t1, a_t|s_t) p(s_t) | p(s_t, a_t) = p(s_t1, a_t|s_t) | p(a_t|s_t)
p(s_t1 | s_t) = \sum p(a_t|s_t) p (s_t1|s_t, a_t)
p(a_t|s_t) = \sum p(s_t1|s_t)p(a_t|s_t, s_t1)
p(s_t1|s_t, a_t) ~ p(s_t1|s_t) p(a_t| s_t)
第二步 closed loop
如果open loop 做好了，closed loop 是自然而然就能做好的吗？
## Adding a Table of Contents

To add a table of contents to a post, simply add

```yml
toc:
  beginning: true
```

to the front matter of the post. The table of contents will be automatically generated from the headings in the post.

### Example of Sub-Heading 1

Jean shorts raw denim Vice normcore, art party High Life PBR skateboard stumptown vinyl kitsch. Four loko meh 8-bit, tousled banh mi tilde forage Schlitz dreamcatcher twee 3 wolf moon. Chambray asymmetrical paleo salvia, sartorial umami four loko master cleanse drinking vinegar brunch. <a href="https://www.pinterest.com">Pinterest</a> DIY authentic Schlitz, hoodie Intelligentsia butcher trust fund brunch shabby chic Kickstarter forage flexitarian. Direct trade <a href="https://en.wikipedia.org/wiki/Cold-pressed_juice">cold-pressed</a> meggings stumptown plaid, pop-up taxidermy. Hoodie XOXO fingerstache scenester Echo Park. Plaid ugh Wes Anderson, freegan pug selvage fanny pack leggings pickled food truck DIY irony Banksy.

### Example of another Sub-Heading 1

Jean shorts raw denim Vice normcore, art party High Life PBR skateboard stumptown vinyl kitsch. Four loko meh 8-bit, tousled banh mi tilde forage Schlitz dreamcatcher twee 3 wolf moon. Chambray asymmetrical paleo salvia, sartorial umami four loko master cleanse drinking vinegar brunch. <a href="https://www.pinterest.com">Pinterest</a> DIY authentic Schlitz, hoodie Intelligentsia butcher trust fund brunch shabby chic Kickstarter forage flexitarian. Direct trade <a href="https://en.wikipedia.org/wiki/Cold-pressed_juice">cold-pressed</a> meggings stumptown plaid, pop-up taxidermy. Hoodie XOXO fingerstache scenester Echo Park. Plaid ugh Wes Anderson, freegan pug selvage fanny pack leggings pickled food truck DIY irony Banksy.

## Table of Contents Options

If you want to learn more about how to customize the table of contents, you can check the [jekyll-toc](https://github.com/toshimaru/jekyll-toc) repository.

### Example of Sub-Heading 2

Jean shorts raw denim Vice normcore, art party High Life PBR skateboard stumptown vinyl kitsch. Four loko meh 8-bit, tousled banh mi tilde forage Schlitz dreamcatcher twee 3 wolf moon. Chambray asymmetrical paleo salvia, sartorial umami four loko master cleanse drinking vinegar brunch. <a href="https://www.pinterest.com">Pinterest</a> DIY authentic Schlitz, hoodie Intelligentsia butcher trust fund brunch shabby chic Kickstarter forage flexitarian. Direct trade <a href="https://en.wikipedia.org/wiki/Cold-pressed_juice">cold-pressed</a> meggings stumptown plaid, pop-up taxidermy. Hoodie XOXO fingerstache scenester Echo Park. Plaid ugh Wes Anderson, freegan pug selvage fanny pack leggings pickled food truck DIY irony Banksy.

### Example of another Sub-Heading 2

Jean shorts raw denim Vice normcore, art party High Life PBR skateboard stumptown vinyl kitsch. Four loko meh 8-bit, tousled banh mi tilde forage Schlitz dreamcatcher twee 3 wolf moon. Chambray asymmetrical paleo salvia, sartorial umami four loko master cleanse drinking vinegar brunch. <a href="https://www.pinterest.com">Pinterest</a> DIY authentic Schlitz, hoodie Intelligentsia butcher trust fund brunch shabby chic Kickstarter forage flexitarian. Direct trade <a href="https://en.wikipedia.org/wiki/Cold-pressed_juice">cold-pressed</a> meggings stumptown plaid, pop-up taxidermy. Hoodie XOXO fingerstache scenester Echo Park. Plaid ugh Wes Anderson, freegan pug selvage fanny pack leggings pickled food truck DIY irony Banksy.
