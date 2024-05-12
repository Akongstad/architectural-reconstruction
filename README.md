# architectural-reconstruction

Reconstruction of architecture from static code | Software Architecture ITU 2024

## Case study project: [Zeeguu API](https://github.com/zeeguu/api)
> **Credits:** The code extends code provided by [Mircae Lungu](https://github.com/mircealungu) for the course **Software Architecture ITU 2024**

This proejct uses [Zeeguu API](https://github.com/zeeguu/api) for a case study of architectural reconstruction from static files. [Zeeguu API](https://github.com/zeeguu/api) is python web api for an elearning study web service.

### View dependency graphs:
The graphs produced by this architectural reconstruction tool are published via GitHub pages at:

**The default graph**
1. Node sizes scale off total degree.
2. Edge thickness scale with total function calls.
3. Edges are directed towards the modules being imported.
4. Hover on nodes to see the times it is imported, the number of imports, and the names of imported modules.
5. Hover edges to see the number of total function calls and distinct function calls to the imported module and a list of functions along with the number of times they are referenced by the module that imports it.
6. Node/edge colors reflect the top level directory they belong to. Zeeguu.core, Zeeguu.api, etc.
7. Use the toolbar below the graph to make dynamic adjustments.

- [Dependency graph with directory abstraction depth 2](https://akongstad.github.io/architectural-reconstruction/dict-depth-2-dep-graph.html)
- [Dependency graph with directory abstraction depth 3](https://akongstad.github.io/architectural-reconstruction/dict-depth-3-dep-graph.html)
- [Dependency graph with directory abstraction depth 4](https://akongstad.github.io/architectural-reconstruction/dict-depth-4-dep-graph.html)
- [Dependency graph with directory abstraction depth all](https://akongstad.github.io/architectural-reconstruction/dict-depth-all-dep-graph.html)

**PageRank graph -- The default graph, but:**
1. It uses the pageRank algorithm to determine node sizes. (Time imported is weighed more highly)

- [Dependency graph with PageRank centrality. Abstraction depth 2](https://akongstad.github.io/architectural-reconstruction/pagerank-dict-depth-2-dep-graph.html)
- [Dependency graph with PageRank centrality. Abstraction depth 3](https://akongstad.github.io/architectural-reconstruction/pagerank-dict-depth-3-dep-graph.html)
- [Dependency graph with PageRank centrality. Abstraction depth 4](https://akongstad.github.io/architectural-reconstruction/pagerank-dict-depth-4-dep-graph.html)
- [Dependency graph with PageRank centrality. Abstraction depth all](https://akongstad.github.io/architectural-reconstruction/pagerank-dict-depth-all-dep-graph.html)

**zeeguu.core graph -- The pagerank graph, but:**
1. Only the zeeguu.core package is shows
2. Colors reflect directories within the zeeguu.core package. Example: zeeguu.core.model, zeeguu.core.util, etc.
   
- [Dependency graph with directory abstraction depth 2. Filtered on zeeguu.core](https://akongstad.github.io/architectural-reconstruction/core-dict-depth-2-dep-graph.html)
- [Dependency graph with directory abstraction depth 3. Filtered on zeeguu.core](https://akongstad.github.io/architectural-reconstruction/core-dict-depth-3-dep-graph.html)
- [Dependency graph with directory abstraction depth 4. Filtered on zeeguu.core](https://akongstad.github.io/architectural-reconstruction/core-dict-depth-4-dep-graph.html)
- [Dependency graph with directory abstraction depth all. Filtered on zeeguu.core](https://akongstad.github.io/architectural-reconstruction/core-dict-depth-all-dep-graph.html)

**Git activity graph -- The default graph, but:**
1. It uses git activity to determine size of nodes.
   
- [Dependency graph with git activity. Abstraction depth 2](https://akongstad.github.io/architectural-reconstruction/churn_dict-depth-2-dep-graph.html)
- [Dependency graph with git activity. Abstraction depth 3](https://akongstad.github.io/architectural-reconstruction/churn_dict-depth-3-dep-graph.html)
- [Dependency graph with git activity. Abstraction depth 4](https://akongstad.github.io/architectural-reconstruction/churn_dict-depth-4-dep-graph.html)
- [Dependency graph with git activity. Abstraction depth 5](https://akongstad.github.io/architectural-reconstruction/churn_dict-depth-5-dep-graph.html)

**AI abstraction for select graphs:**

- [GPT4-turbo summary of depth 2 graph](https://github.com/Akongstad/architectural-reconstruction/blob/main/public/ai-depth-2.md) of: [Dependency graph with directory abstraction depth 2](https://akongstad.github.io/architectural-reconstruction/dict-depth-2-dep-graph.html)
- [GPT4-turbo summary of depth 3 graph](https://github.com/Akongstad/architectural-reconstruction/blob/main/public/ai-depth-3.md) of: [Dependency graph with directory abstraction depth 3](https://akongstad.github.io/architectural-reconstruction/dict-depth-3-dep-graph.html)
- [GPT4-turbo summary of graph with page rank nodes depth 4](https://github.com/Akongstad/architectural-reconstruction/blob/main/public/ai-pagerank-4.md) of: [Dependency graph with PageRank. Abstraction depth 4](https://akongstad.github.io/architectural-reconstruction/pagerank-dict-depth-4-dep-graph.html)
- [GPT4-turbo summarty of graph with git activity depth 3](https://github.com/Akongstad/architectural-reconstruction/blob/main/public/ai-churn-depth-3.md) of:  [Dependency graph with git activity. Abstraction depth 3](https://akongstad.github.io/architectural-reconstruction/churn_dict-depth-3-dep-graph.html)
- [GPT4-turbo summary of zeeguu.core graph depth 3](https://github.com/Akongstad/architectural-reconstruction/blob/main/public/ai-core-depth-3.md) of: [Dependency graph with directory abstraction depth 3. Filtered on zeeguu.core](https://akongstad.github.io/architectural-reconstruction/core-dict-depth-3-dep-graph.html)
- [GPT4-turbo summary zeeguu.core graph depth 4 ](https://github.com/Akongstad/architectural-reconstruction/blob/main/public/ai-core-depth-4.md) of: [Dependency graph with directory abstraction depth 4. Filtered on zeeguu.core](https://akongstad.github.io/architectural-reconstruction/core-dict-depth-4-dep-graph.html)

## Links

1. Lecture notes: <https://github.com/mircealungu/reconstruction>
2. Assignment: <https://docs.google.com/document/d/10bTyUS4ZocReS3j2AxHak_-rBh_Yv_0NM6XDQrt0YkY/edit#heading=h.yopcbjqrxgwj>
3. Zeeguu API: <https://github.com/zeeguu/api>
4. Zeeguu frontend: <https://github.com/zeeguu/web>
5. Report: <https://www.overleaf.com/project/6633aa8b62ad154eebc87df2>

### Papers

1. [1] Symphony: View-Driven Software Architecture Reconstruction <https://ipa.win.tue.nl/archive/springdays2005/Deursen1.pdf>
2. [2] [Demeyer et al., Object Oriented Reengineering Patterns (Chapter 1.2)](https://www.oscar.nierstrasz.org/files/oorp/OORP-2013-11-27.pdf)
3. [3] [What architects should know about reverse engineering and reengineering](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=05981602215076b7492b87a8a1f7157dcc9c2196) R. Koschke, In 5th Working IEEE/IFIP Conference on Software Architecture (WICSA'05)_(pp. 4-10). IEEE. 
