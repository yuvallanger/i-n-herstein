# I. N. Herstein’s Topics in Algebra 2nd Edition

## Prove: A = (A and B) or (A - B)

### A and B = null

A = (A and B) or (A - B)
  = null or (A - B)
  = (A - B)
  = {x in A | x not in B}  -- Because x in A is never x in B, this is true for every x in A
  = {x in A}
  = A

### A and B is proper subset of A or B

A = (A and B) or (A - B)
  = (A or (A - B)) and (B or (A - B))
  = (A or {x in A | x not in B}) and
    (B or {x in A | x not in B})
  = (A or {x in A | x not in B}) and  -- A or a subset of A = A
    (B or {x in A | x not in B})  -- (B or (subset of A which is not shared with B) = (A or B) [because B also holds the subset which is shared with A]
  = A and (B or A)
  = (A and B) or (A and A)
  = (A and B) or A  -- the subset of A that is shared with B is a subset of A, so a union of a subset of A with A, is A.
  = A

### A is a proper subset of B

A = (A and B) or (A - B)
  = A or (A - B)
  = A

### B is a proper subset of A

A = (A and B) or (A - B)
  = B or (A - B)  -- the union of the subset of A that is not shared with B and B will be A
  = A

### A = B

A = (A and B) or (A - B)
  = A or null
  = A
