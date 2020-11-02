---
title: Number of Digits
sidebar: mydoc_sidebar
permalink: recursion_numberofdigits.html
folder: recursion
keywords: algorithm recursion numberofdigits
tags: [algorithm, recursion, numberofdigits]
last_updated: November 02, 2020
---

{% include callout.html content="<strong>Problem:</strong><br/> Given a number n, find the count of digits in n." type="primary" %} 

## Solution

```csharp
public int NumberOfDigits(int num)
{
    if (num < 10)
        return 1;
    else
    {
        return 1 + NumberOfDigits(num / 10);
    }
}
```

| Complexity | Value |
|-------|--------|
| Time | O(logN) |
| Space | O(logN) |

{{site.data.alerts.note}}
<br/>
<pre>
1234 / 10 = 123 => coefficient
1234 % 10 = 4   => remainder
</pre>
{{site.data.alerts.end}}


