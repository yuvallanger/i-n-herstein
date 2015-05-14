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
  if x not in A and x not in B
    x not in (A cap B)
    x not in (A - B)
    x not in ((A cap B) cup (A - B))
    i.e., this case never happens
  if x not in A and x in B
    x not in (A cap B)
    x not in (A - B)
    x not in ((A cap B) cup (A - B))
    i.e., this case never happens
  if x in A and x not in B
    x not in (A cap B)
    x in (A - B)
    x in (A cap B) cup (A - B)
  if x in A and x in B
    x in (A cap B)
    x in (A - B)
    x in ((A cap B) cup (A - B))
  the only truthful cases are those that maintain that x in A
