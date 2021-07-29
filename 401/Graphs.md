# Graphs:
A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

Here is some common terminology used when working with Graphs:

Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
Edge - An edge is a connection between two nodes.
Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
Degree - The degree of a vertex is the number of edges connected to that vertex.

![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)


A Graph consists of a finite set of vertices(or nodes) and set of Edges which connect a pair of nodes.

In the above Graph, the set of vertices V = {0,1,2,3,4} and the set of edges E = {01, 12, 23, 34, 04, 14, 13}.

Graphs are used to solve many real-life problems. Graphs are used to represent networks. The networks may include paths in a city or telephone network or circuit network. Graphs are also used in social networks like linkedIn, Facebook. For example, in Facebook, each person is represented with a vertex(or node). Each node is a structure and contains information like person id, name, gender, locale etc.

# Types of graphs:

* Undirected Graph

![img](https://www.researchgate.net/profile/Hakan-Terelius/publication/265428782/figure/fig3/AS:669498856194058@1536632374537/An-undirected-graph-with-7-nodes-and-7-edges.png)

* Directed Graph

![img](https://www.researchgate.net/profile/John-Lee-156/publication/220863116/figure/fig1/AS:669516962988037@1536636691241/An-example-of-a-directed-graph-with-9-nodes.png)

# Types of Graph Representations:

* Adjacency List

![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

* Adjacency Matrix

![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/AdjMatrix.PNG)

## example:

```
ALGORITHM BreadthFirst(vertex)
    DECLARE nodes <-- new List()
    DECLARE breadth <-- new Queue()
    DECLARE visited <-- new Set()

    breadth.Enqueue(vertex)
    visited.Add(vertex)

    while (breadth is not empty)
        DECLARE front <-- breadth.Dequeue()
        nodes.Add(front)

        for each child in front.Children
            if(child is not visited)
                visited.Add(child)
                breadth.Enqueue(child)   

    return nodes;

```