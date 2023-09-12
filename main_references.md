# Titulo: ANÁLISIS DE TÉCNICAS DE OPTIMIZACIÓN PARA PIPELINES EN REPOSITORIOS DE ALMACENAMIENTO DE DATOS DE GRAN ESCALA #

# Objetivo General: Generar un modelo de implementación de buenas prácticas a partir del estudio de pipelines en repositorios de datos en sistemas de gran escala (Big Data, Data Lakes, Data Warehouse) para mejorar su rendimiento #

# Performance Tuning and Optimization of Apache Spark Applications. #

```
Ninan, A. (2023). Performance Tuning and Optimization of Apache Spark Applications. International Journal of Computer Trends and Technology, 71(5), 10–14. https://doi.org/10.14445/22312803/IJCTT-V71I5P103
```

## Summary ## 

The research article explores optimization techniques for Apache Spark applications and aims to help users maximize resource utilization, minimize execution time, and improve overall application efficiency. The paper provides an overview of Apache Spark's architecture, data structures, core components, and execution model. It also discusses performance-related parameters such as data partitioning, data serialization, caching strategies, executor configuration, memory management, and garbage collection settings.

Advanced optimization techniques like adaptive query execution, dynamic allocation, and data locality are discussed in detail.

This study is a comprehensive guide to performance tuning and optimization for Apache Spark applications, aiming to empower users to harness the full potential of this powerful data processing engine, unlock new insights from their big data workloads, and save on costs.

# Relevance to the Research Topic

- Performance factors
- Advanced Optimization techniques
- Spark Architecture Description (Shallow)

# Spark: Cluster Computing with Working Sets #

```
Zaharia, M., Chowdhury, M., Franklin, M. J., Shenker, S., & Stoica, I. (2010, June). Spark: Cluster Computing with Working Sets. 2nd USENIX Workshop on Hot Topics in Cloud Computing (HotCloud 10). https://www.usenix.org/conference/hotcloud-10/spark-cluster-computing-working-sets
```

## Summary ##

The research article discusses about Spark, which supports data-intensive applications while maintaining the scalability and fault tolerance of MapReduce. The authors identify that most existing systems are built around an acyclic data flow model that is not suitable for all applications, particularly those that reuse a working set of data across multiple parallel operations.

To address this, Spark introduces an abstraction called resilient distributed datasets (RDDs), a read-only collection of objects partitioned across a set of machines that can be rebuilt if a partition is lost. RDDs are more efficient than MapReduce for iterative machine learning jobs and interactive data analysis tools. The paper demonstrates that Spark can outperform Hadoop by 10x in iterative machine learning jobs and can interactively query a large dataset with sub-second response time.

Also its discussed how Spark provides two main abstractions for parallel programming: resilient distributed datasets and parallel operations on these datasets. Additionally, Spark supports two types of shared variables, broadcast variables and accumulators, to support common usage patterns.

# Relevance to the Research Topic

- Origin of Apache Spark
- Why Spark and what made it special at the beginning
- Execution plan


# A Methodology for Spark Parameter Tunning"

```
Gounaris, A., & Torres, J. (2018). A Methodology for Spark Parameter Tuning. Big Data Research, 11, 22–32. https://doi.org/10.1016/J.BDR.2017.05.001
```

# Summary of the Research Article

The research article discusses aabout a systematic methodology to tune over 150 configurable parameters in Spark. The authors recognize that while Spark's default values allow developers to quickly deploy their applications, there is potential for performance improvement.

The paper investigates the impact of the most important tunable Spark parameters related to shuffling, compression, and serialization on application performance.

The researchers propose an alternative systematic methodology for parameter tuning that can be easily applied to any computing infrastructure.

The main contribution of this work is the proposed systematic methodology for parameter tuning which has shown speedups starting from 20% in validating test case studies.

# Relevance to the Research Topic

- Generalization of tuning parameters for different architectures and datasets
- More relevant parameters for performance (in execution times) based on prev literature



# An Approach for Optimizing the Performance for Apache Spark Applications #

```
Gupta, P., Sharma, A., & Jindal, R. (2018). An approach for optimizing the performance for apache spark applications. 2018 4th International Conference on Computing Communication and Automation, ICCCA 2018. https://doi.org/10.1109/CCAA.2018.8777541
```

# Summary of the Research Article

The research article discusses various techniques to optimize the performance of Spark applications. The authors identify that the default parameters of Spark may not provide optimal solutions for every configuration and environment, hence tuning these parameters is crucial.

The paper explores several parameters/options such as caching, broadcast variables, repartitioning, and number of executors that can be tuned according to the environment for improved performance. The authors conducted an experiment with a content recommender system application and found significant improvements in execution time by optimizing these parameters.

# Relevance to the research Topic

- Conclussons of the research:
    1. **Dataframe Caching**: Caching dataframes resulted in a 37% reduction in execution time.
    2. **Broadcast Variables**: Using broadcast join reduced the execution time by approximately 9%.
    3. **Increasing Number of Partitions**: Increasing the number of partitions and cores led to a 67% reduction in execution time.
    4. **Optimizing Number of Executors**: By optimizing the number of executors and data partitions based on data volume, number of cluster nodes, available cores and executor memory, the authors achieved a 78% reduction in execution time.

    The authors concluded that combining all these optimization techniques could lead to an 87% reduction in execution time for the content recommender system application.
