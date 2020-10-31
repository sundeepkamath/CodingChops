---
title: Absolute
sidebar: mydoc_sidebar
permalink: math_absolute.html
folder: math
keywords: algorithm math absolute
tags: [algorithm, math, absolute]
last_updated: October 31, 2020
---

{% include callout.html content="<strong>Problem:</strong><br/> You are given an interger I. You need to print the absolute value of the interger I." type="primary" %} 

## Solution

```csharp
public int AbsoluteValue(int input)
{
    if (input < 0)
        return input * -1;

    return input;
}
```

| Complexity | Value |
|-------|--------|
| Time | O(1) |
| Space | O(1) |
