# leetcode 896 - Monotonic Array

## Java
```Java
public bool IsMonotonic(int[] A)
{   
    var monoIncreasing = true;
    var monoDescreasing = true;
    for (int i = 0; i < A.length - 1; ++i)
    {
        if (A[i] > A[i + 1])
            monoIncreasing = false;
        if (A[i] < A[i + 1])
            monoDescreasing = false;
        if (monoIncreasing == false && monoDescreasing == false) break;
    }

    return monoIncreasing || monoDescreasing;
}
```

## C#
```C#
public bool IsMonotonic(int[] A)
{   
    var monoIncreasing = true;
    var monoDescreasing = true;
    for (int i = 0; i < A.Length - 1; ++i)
    {
        if (A[i] > A[i + 1])
            monoIncreasing = false;
        if (A[i] < A[i + 1])
            monoDescreasing = false;
        if (increasing == false && monoDescreasing == false) break;
    }

    return monoIncreasing || monoDescreasing;
}
```
