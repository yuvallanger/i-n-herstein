# I. N. Herstein’s Topics in Algebra 2nd Edition

## Prove: A = (A cap B) cup (A - B)

### LHS => RHS

for each x in A
   if x in B
     x in (A cap B)
     x in ((A cap B) cup (A - B))
   if x not in B
     x in (A - B)
     x in ((A cap B) cup (A - B))

### RHS => LHS

for each x in ((A cap B) cup (A - B))
  if x in (A cap B)
    x in A and x in B
  if x in (A - B)
    x in A and x not in B
  i.e. for both cases we see:
    (x in A and x in B) or (x in A and x not in B)
  logical manipulation gives us that for both cases:
    x in A
