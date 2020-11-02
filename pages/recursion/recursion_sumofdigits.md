---
title: Sum of Digits
sidebar: mydoc_sidebar
permalink: recursion_sumofdigits.html
folder: recursion
keywords: algorithm recursion sumofdigits
tags: [algorithm, recursion, sumofdigits]
last_updated: November 02, 2020
---

{% include callout.html content="<strong>Problem:</strong><br/> Given a number n, find the sum of digits of n" type="primary" %} 

## Solution

```csharp
public int SumOfDigits(int num)
{
    if (num < 10)
        return 1;
    else
    {
        return 1 + SumOfDigits(num / 10);
    }
}
```

| Complexity | Value |
|-------|--------|
| Time | O(logN) |
| Space | O(logN)(recursive) |

{{site.data.alerts.note}}
<br/>
<pre>
1234 / 10 = 123 => coefficient
1234 % 10 = 4   => remainder
</pre>
{{site.data.alerts.end}}


