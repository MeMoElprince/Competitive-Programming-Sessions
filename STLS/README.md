# STLS Content 

> Session Video
- **[session]()**

> Other Videos
- **[Adel Nasim (Vector-part1)](https://www.youtube.com/watch?v=AMnultLTdlI&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=2)**
- **[Adel Nasim (Vector-part2)](https://www.youtube.com/watch?v=4b3Glt6zWY4&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=3&t=9s)**
- **[Adel Nasim (Vector-part3)](https://www.youtube.com/watch?v=4om6SL_cF50&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=4)**
- **[Adel Nasim (Deque)](https://www.youtube.com/watch?v=PPFhtX23oXc&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=5)**
- **[Adel Nasim (List)](https://www.youtube.com/watch?v=U2oXdm4PfeQ&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=6)**
- **[Adel Nasim (Forward List)](https://www.youtube.com/watch?v=hp7BCTdEDFs&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=7)**
- **[Adel Nasim (Pair)](https://www.youtube.com/watch?v=ucQnEO0MSSs&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=8)**
- **[Adel Nasim (set)](https://www.youtube.com/watch?v=Yg7dpbXhhlY&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=9&t=6s)**
- **[Adel Nasim (Map-part1)](https://www.youtube.com/watch?v=cQ5psV2P2iU&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=11&t=1s)**
- **[Adel Nasim (Map-part2)](https://www.youtube.com/watch?v=rWnu4r8fubk&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=11)**
- **[Adel Nasim (Unordered Set/Multiset)](https://www.youtube.com/watch?v=m9t4ORIMCro&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=13)**
- **[Adel Nasim (Unordered Map/Multimap)](https://www.youtube.com/watch?v=q2ytLwNbR4w&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=13)**
- **[Adel Nasim (Stack)](https://www.youtube.com/watch?v=9r7IDtX5KS4&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=14&t=1s)**
- **[Adel Nasim (Queue)](https://www.youtube.com/watch?v=iLJXB9Daeq8&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=15)**
- **[Adel Nasim (Priority Queue)](https://www.youtube.com/watch?v=0zr0JqSw7ic&list=PLCInYL3l2AainAE4Xq2kdNGDfG0bys2xp&index=16&t=2s)**

> Problems (codeforces)
- **[H1. Maximum Crossings (Easy Version)](https://codeforces.com/contest/1676/problem/H1)**
- **[H2. Maximum Crossings (Hard Version)](https://codeforces.com/contest/1676/problem/H2)**
- **[A. Cakes](https://codeforces.com/group/9PTNrhBNKn/contest/337624/problem/A)**
- **[ZB. Subarray Sums II](https://codeforces.com/gym/102961/problem/ZB)**
- **[E. repair Harry Potter wand](https://codeforces.com/group/p6hc42ieQe/contest/336575/problem/E)**
- **[J. Next Element](https://codeforces.com/group/c3FDl9EUi9/contest/263096/problem/J)**
- **[STLS sheet](https://codeforces.com/group/KQlzWufN6x/contest/376252)**

## Topic ... Ordered Set

> It performs all the operations as performed by the set data structure in STL in log(n) complexity.
 And performs two additional operations also in log(n) complexity .
 - **order_of_key (k) :**  Number of items strictly smaller than k .
 - **find_by_order(k) :**  K-th element in a set (counting from zero).

> Required header files to implement ordered set.

>Template
```
  #include <ext/pb_ds/assoc_container.hpp>
  #include <ext/pb_ds/tree_policy.hpp>
  #using namespace __gnu_pbds;
  #define orderedSet tree < int ,  null_type ,  less ,  rb_tree_tag ,  tree_order_statistics_node_update >
```
> `tree < int ,  null_type ,  less ,  rb_tree_tag ,  tree_order_statistics_node_update >`
- **int :** It is the type of the data that we want to insert (KEY).It can be integer, float or pair of int etc.
- **null_type :** It is the mapped policy. It is null here to use it as a set.If we want to get map but not the set, as the second argument type must be used mapped type.
- **less :** It is the basis for comparison of two functions.
- **rb_tree_tag :** type of tree used. It is generally Red black trees because it takes log(n) time for insertion and deletion while other take linear time such as splay_tree.
- **tree_order_statistics_node__update :** It is included in tree_policy.hpp and contains various operations for updating the node variants of a tree-based container, so we can keep track of metadata like the number of nodes in a subtree

## Topic ... Ordered MultiSet

> The difference between ordered set and ordered multiset is in the comparison funtion.
- **less :** unique elements sorted in non-decreasing order.
- **less_equal :** non-unique elements sorted in non-decreasing order.
- **greater :** unique elements sorted in non-increasing order.
- **greater_equal :** non-unique elements sorted in non-increasing order.
