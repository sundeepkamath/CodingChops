---
title: Factorial
sidebar: mydoc_sidebar
permalink: math_factorial.html
folder: math
keywords: algorithm math factorial
tags: [algorithm, math, factorial]
last_updated: October 31, 2020
---

{% include callout.html content="<strong>Problem:</strong><br/> Given a positive integer N, find factorial of N." type="primary" %} 

## Solution 1

```csharp
public int Factorial(int val)
{
    if (val == 0 || val == 1)
        return 1;

    return val * Factorial(val - 1);
}
```
{{site.data.alerts.note}}
Factorial can be calculated using ...
<pre>
n! = n * (n-1)! <br/>
n! = 1 if n = 0 or n = 1  <br/>
</pre>
Answer should be in long as it may overflow the int.<br/>

Also, calculating factorial recursively can be costly. Hence, its better to use the iterative solution." 
{{site.data.alerts.end}}

## Solution 2

```csharp
public long Factorial(int val)
{
    long ans = 1;

    for (int i = 2; i <= val; i++)
        ans = ans * i;

    return ans;
}
```

| Complexity | Value |
|-------|--------|
| Time | O(n) |
| Space | O(1) |
