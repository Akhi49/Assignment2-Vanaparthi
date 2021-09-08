# AKHILVANAPARTHI
###### Grandparents house
my favorite place is my **grand parenrts home**,it is located in **Telangana India**.
The place is perfect with a good and peacfull weather,i mostly go near a small
lake for fishing and we do swim,every festival is celebrated  colorfully.
*******************
# TRAVELLING

1. Bus to Kansas City

    1. fly to Toronto    
    2. train

4. UP Express Pearson Airport

3. Toronto Union Station

4. Niagara Falls GO

>Nested!

### list of resources needed
* swim suit

    * EXTRA

- extra clothes

- water bottels

- Camera

- medicine in emergency kit

***Link to About me*** 
<https://github.com/Akhi49/Assignment2-Vanaparthi/blob/main/AboutMe.md>

********************************************************

# FOOD AND DRINKS!!
This table shows you the food and drinks to try in **NWMSU** student union.
| food/drinks | Location | Amount |
| --- | --- | ---: |
| Chicken Sandwich | Chick-fil-A | $5 |
| Grilled Nuggets | Chick-fil-A | $14-$15 |
| Brisket Egg Sandwich | Einstein Bros. Bagels | $7 |
| iced caramel macchiato | Starbucks | $5 |

****************************************************
### Quotes


> The future belongs to those who believe in the beauty of their dreams. 

 *-Eleanor Roosevelt*

 

> "Spread love everywhere you go. Let no one ever come to you without leaving happier."

 *-Mother Teresa*
 

 *************************************************
 ### Code Fencing

 

 > A group of edges that connects two set of vertices in a graph is called cut in graph theory. So, at every step of Prim’s algorithm, we find a cut (of two sets, one contains the vertices already included in MST and other contains rest of the vertices), pick the minimum weight edge from the cut and include this vertex to MST Set.

 <https://www.geeksforgeeks.org/prims-minimum-spanning-tree-mst-greedy-algo-5/>

```int
int n;
vector<vector<int>> adj; // adjacency matrix of graph
const int INF = 1000000000; // weight INF means there is no edge
struct Edge {
    
    int w = INF, to = -1;
};
```
void prim() {
    int total_weight = 0;
    vector<bool> selected(n, false);
    vector<Edge> min_e(n);
    min_e[0].w = 0;
    ```
   ```
    for (int i=0; i<n; ++i) {
        int v = -1;
        for (int j = 0; j < n; ++j) {
            if (!selected[j] && (v == -1 || min_e[j].w < min_e[v].w))
                v = j;
        }
        
        if (min_e[v].w == INF) {
            cout << "No MST!" << endl;
            exit(0);
        }
        
        selected[v] = true;
        total_weight += min_e[v].w;
        if (min_e[v].to != -1)
            cout << v << " " << min_e[v].to << endl;
       
        for (int to = 0; to < n; ++to) {
            if (adj[v][to] < min_e[to].w)
                min_e[to] = {adj[v][to], v};
        }
    }
    count
    cout << total_weight << endl;
}
```

<https://cp-algorithms.com/graph/mst_prim.html>

