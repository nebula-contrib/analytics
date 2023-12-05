# 大型分布式图计算系统的图算法开发  -  OSPP2023

在 Plato 系统上实现 PersonalizedPageRank(个性化pagerank)、TrustRank（信任指数）、BeliefPropagation（置信度传播）三个图算法。

## Personalized PageRank 算法
* 核心算法文件: `plato/algo/ppr/personalized_pagerank.hpp`  
* 算法 CLI 应用文件: `example/personalized_pagerank.cc`
* 算法运行脚本: `scripts/run_ppr_local.sh`
* 基于 PUSH-PULL 切换优化的算法版本: `example/pushpull_ppr.cc` 和 `scripts/run_pushpull_ppr_local.sh`
* 算法正确性验证: 参照 [Spark-GraphX](https://github.com/apache/spark/blob/master/graphx/src/main/scala/org/apache/spark/graphx/lib/PageRank.scala) 和 [Neo4j PageRank](https://neo4j.com/docs/graph-data-science/current/algorithms/page-rank/) 相关实现

## TrustRank 算法
* 核心算法文件: `plato/algo/trustrank/trustrank.hpp`  
* 算法 CLI 应用文件: `example/trustrank.cc`
* 算法运行脚本: `scripts/run_trustrank_local.sh`
* 算法正确性验证: 参照 [TrustRank 论文](https://dl.acm.org/doi/10.5555/1316689.1316740) 及 [bhaveshgawri/PageRank](https://github.com/bhaveshgawri/PageRank/blob/master/TrustRank.py) 相关实现

## Belief Propagation 算法
* 核心算法文件: `plato/algo/bp/belief_propagation.hpp`  
* 算法 CLI 应用文件: `example/belief_propagation.cc`
* 算法运行脚本: `scripts/run_bp_local.sh`
* 算法正确性验证: 参照 [HewlettPackard/sandpiper](https://github.com/HewlettPackard/sandpiper) 和 [mbforbes/py-factorgraph](https://github.com/mbforbes/py-factorgraph) 相关实现