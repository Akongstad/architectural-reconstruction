# architectural-reconstruction

Reconstruction of architecture from static code | Software Architecture ITU 2024

## Case study project: [Zeeguu API](https://github.com/zeeguu/api)
> **Credits:** The code extends code provided by [Mircae Lungu](https://github.com/mircealungu) for the course **Software Architecture ITU 2024**

This proejct uses [Zeeguu API](https://github.com/zeeguu/api) for a case study of architectural reconstruction from static files. [Zeeguu API](https://github.com/zeeguu/api) is python web api for an elearning study web service.

**AI abstraction for select graphs:**

**View dependency graphs:** The graphs produced by this architectural reconstruction tool are published via github pages at:

- [Dependency graph with directory abstraction depth 2](https://akongstad.github.io/architectural-reconstruction/dict-depth-2-dep-graph.html)
- [Dependency graph with directory abstraction depth 3](https://akongstad.github.io/architectural-reconstruction/dict-depth-3-dep-graph.html)
- [Dependency graph with directory abstraction depth 4](https://akongstad.github.io/architectural-reconstruction/dict-depth-4-dep-graph.html)
- [Dependency graph with directory abstraction depth all](https://akongstad.github.io/architectural-reconstruction/dict-depth-all-dep-graph.html)

*Zeeguu.core focus*

- [Dependency graph with directory abstraction depth 2. Filtered on zeeguu.core](https://akongstad.github.io/architectural-reconstruction/core-dict-depth-2-dep-graph.html)
- [Dependency graph with directory abstraction depth 3. Filtered on zeeguu.core](https://akongstad.github.io/architectural-reconstruction/core-dict-depth-3-dep-graph.html)
- [Dependency graph with directory abstraction depth 4. Filtered on zeeguu.core](https://akongstad.github.io/architectural-reconstruction/core-dict-depth-4-dep-graph.html)
- [Dependency graph with directory abstraction depth all. Filtered on zeeguu.core](https://akongstad.github.io/architectural-reconstruction/core-dict-depth-all-dep-graph.html)

*With node size based on PageRank centrality*

- [Dependency graph with PageRank centrality. Abstraction depth 2](https://akongstad.github.io/architectural-reconstruction/pagerank-dict-depth-2-dep-graph.html)
- [Dependency graph with PageRank centrality. Abstraction depth 3](https://akongstad.github.io/architectural-reconstruction/pagerank-dict-depth-3-dep-graph.html)
- [Dependency graph with PageRank centrality. Abstraction depth 4](https://akongstad.github.io/architectural-reconstruction/pagerank-dict-depth-4-dep-graph.html)
- [Dependency graph with PageRank centrality. Abstraction depth all](https://akongstad.github.io/architectural-reconstruction/pagerank-dict-depth-all-dep-graph.html)

*With node size based on git activity:*

- [Dependency graph with git activity. Abstraction depth 2](https://akongstad.github.io/architectural-reconstruction/churn_dict-depth-2-dep-graph.html)
- [Dependency graph with git activity. Abstraction depth 3](https://akongstad.github.io/architectural-reconstruction/churn_dict-depth-3-dep-graph.html)
- [Dependency graph with git activity. Abstraction depth 4](https://akongstad.github.io/architectural-reconstruction/churn_dict-depth-4-dep-graph.html)
- [Dependency graph with git activity. Abstraction depth 5](https://akongstad.github.io/architectural-reconstruction/churn_dict-depth-5-dep-graph.html)

**Tips: Color depends on top level package. Hover node to see imported modules. Hover edges to see function call information.**

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
