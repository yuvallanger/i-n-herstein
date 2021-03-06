# I. N. Herstein’s Topics in Algebra 2nd Edition

Thanks effex for recommending this book.

Mirrors at:

* [Gitlab][gitlab-mirror]
* [Github][github-mirror]

## Chapter 1

### Page 5 - Prove: A = (A cap B) cup (A - B)

(thanks Z-module)

#### LHS => RHS

```
for each x in A
   if x in B
     x in (A cap B)
     x in ((A cap B) cup (A - B))
   if x not in B
     x in (A - B)
     x in ((A cap B) cup (A - B))
```

#### RHS => LHS

```
for each x in ((A cap B) cup (A - B))
  if x in (A cap B)
    x in A and x in B
  if x in (A - B)
    x in A and x not in B
  i.e. for both cases we see:
    (x in A and x in B) or (x in A and x not in B)
  logical manipulation gives us that for both cases:
    x in A
```

### Page 7 - Prove Example 1.1.3

(thanks math718)

```
n is integer and greater than one.
a ~ b if a - b is a multiple of n.
```

#### a ~ a

```
k = 0

a - a = 0 = k * n
```

#### a ~ b => b ~ a

```
a - b = k * n

b - a = -(a - b)
      = -(k * n)
      so, b ~ a
```

#### a ~ b and b ~ c => a ~ c

(thanks effex)

```
a - b = r * n

b - c = s * n

a - c = (a - b) + (b - c)
      = r * n + s * n
      = (r + s) * n
```

[gitlab-mirror]: <https://gitlab.com/yuvallanger/i-n-herstein.git>
[github-mirror]: <https://github.com/yuvallanger/i-n-herstein.git>
