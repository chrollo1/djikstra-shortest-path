# Djikstra's Shortest Path Algorithm

Given a directed graph G = (V, E) with positive edge weights, the single-source shortest path problem can be solved using Djikstra's shortest path algorithm.

The time complexity of such is: 
O(m log n)


```
**method** dis[] djikstra(Graph, src):
  dis[src] := 0
  for each vertex v in Graph:
    if v = src
      dis[v] := integer.max
    add v to q
    
  while q is not empty:
    v := vertex in q with min dis[v]
    remove v from q
    
    for each neighbour u of v:
      alt := dis[v] + len(v,u)
      if alt < dis[u]:
        dis[u] := alt
        
  return dis[]
```

