---
layout: post
title: "Matplotlib-Simple_Graph"
comments: true
description: "Simple_Graph"
keywords: "Matplotlib"
tags : 
- Matplotlib
- Python
- iPython
---


### Code

{% highlight python linenos %}
import numpy as np
import matplotlib.pyplot as plt
x = np.arange(0, 6, 0.1);
y = np.sin(x)
plt.plot(x, y)
{% endhighlight %}
![실행 스크린샷]({{ site.url }}/assets/images/2017-04-26/Simple_Graph.png)

[ipython 파일]({{ site.url }}/assets/file/2017-04-26/Simple_Graph.ipynb)

공식 문서 링크 : [matplotlib.pyplot](http://matplotlib.org/2.0.0/api/pyplot_api.html)
