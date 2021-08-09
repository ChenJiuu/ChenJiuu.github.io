---
layout: post
title:  "ImportError when installing ccpem"
date:   2021-08-09 16:01:48 +0900
categories: blogs
---

When installing ccpem suite, an error like:
{% highlight ruby %}
ImportError: /lib/x86_64-linux-gnu/libfontconfig.so.1: undefined symbol: FT_Done_MM_Var
{% endhighlight ruby %}
may appear.
 
This error has been documented on `https://www.ccpem.ac.uk/user_help/known_issues.php`.
In brief, `rm $CCPEM/lib/libfreetype.so*`  would help.