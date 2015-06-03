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

#### Page 8 to 9 - Problems

##### 1. a. Prove: $(A\subset B)\wedge (B\subset C)\implies A\subset C$

$S\subset T\iff x\in S\implies x\in T$.

According to this definition, the above can be rewritten as:

$x\in A\implies B\wedge x\in B\implies x\in C$

b. Prove $B\subset A\implies A\cup B=A$, and conversely.

(1) $B\subset A\iff x\in B\implies x\in A$

(2) $A\cup B={x|x\in A\vee x\in B}$

$$
let x\in A, \newline
  then x\in A\vee x\in B \newline
let x\in B,
  then, according to (1), \implies x\in A\implies x\in A\vee x\in B
$$

conversely, 

Prove: A\cup (B\cap C)=(A\cup B)\cap (A\cup C)

A\cup (B\cap C)
 \implies {y|y\in A or y in {x| x in B and x in C}}
 \implies {y|y\in A or (y in B and y in C)}
 \implies {y|(y\in A or y in B) and (y in A or y in C)}
 \implies (A\cup B) cap (A cup C) A cup (B cap C)
 \implies {y|y in A or y in {x|x in B and x in C}}
 \implies {y|y in A or (y in B and y in C)}
 \implies {y|(y in A or y in B) and (y in A or y in C)}
 \implies (A cup B) cap (A cup C)

(A\cup B)\cap (A\cup C)
  \implies {x|x\in A\vee x\in B}\cap {x|x\in A\vee x\in C}
  \implies {y|y\in {x|x\in A\vee x\in B}\wedge y\in {x|x\in A\vee x\in C}}
  \implies {y|(y\in A\vee x\in B)\wedge (y\in A\vee y\in C)}
  \implies {y|y\in A\vee (y\in B\wedge y\in C)}
  \implies {y|y\in A\vee y\in {x|x\in B\wedge x\in C}}
  \implies {y|y\in A\vee y\in (B\cap C)}
  \implies A\cup (B\cap C)


(A\cap B)’=A’\cup B’

(A\cap B)’
  \implies S-(A\cap B)
  \implies {x|x\in S\wedge not (x\in (A\cap B))}
  \implies {x|x\in S\wedge not (x\in A\wedge x\in B))}
  \implies {x|x\in S\wedge ((not x\in A)\vee (not x\in B))}
  \implies {x|(x\in S\wedge (not x\in A))\vee (x\in S\wedge (not x\in B))}
  \implies {x|x\in A’\vee x\in B’}
  \implies A’\cup B’


(A\cup B)’=A’\cap B’


[gitlab-mirror]: <https://gitlab.com/yuvallanger/i-n-herstein.git>
[github-mirror]: <https://github.com/yuvallanger/i-n-herstein.git>
