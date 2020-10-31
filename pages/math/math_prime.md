---
title: Prime
sidebar: mydoc_sidebar
permalink: math_prime.html
folder: math
keywords: algorithm math prime
tags: [algorithm, math, prime]
last_updated: October 31, 2020
---

{% include callout.html content="<strong>Problem:</strong><br/> Check if a give number N is a prime number" type="primary" %} 

## Solution

```csharp
public bool IsPrime(int num)
{
    if (num <= 1)
        return false;

    for (int i = 2; i <= System.Math.Sqrt(num); i++)
    {
        if (num % i == 0)
            return false;
    }

    return true;
}
```

| Complexity | Value |
|-------|--------|
| Time | O(n<sup>1/2</sup>) |
| Space | O(1) |

{{site.data.alerts.note}}
<br/>A prime number is a whole number greater than 1, which is only divisible by 1 and itself. <br/>
For example: 2 3 5 7 11 13 17 19 23 ........<br/>
An optimal way to do this is to iterate from 2 to sqrt(n) as the factors from 2 to sqrt(n) have multiples from sqrt(n)+1 to n. So, by iterating till sqrt(n) only, we can check if a number is prime.
{{site.data.alerts.end}}


