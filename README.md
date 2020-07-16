# The Open Source AI Handbook

* [Preface](preface)
  * [Who This Book Is For](preface/who_this_book_is_for.md)
  * Conventions Used in This Book
  * Using Code Examples
  * IBM Online Learning
  * How to Contact Us
  * Acknowledgments

* The self-service data science reference architecture  
Description: This chapter introduces the open source data science platform and their components
  * Motivation
  * Components
    * Virtualization: Kubernetes and OpenShift, AKS(?)
    * Data Marts: PostgreSQL
    * Storage Layer/Data Lake: Ceph, S3, Cloud Object Store
    * Data Integration: Apache Spark
    * Dashboarding: Apache Superset, R Shiny
    * IDE: Jupyther Hub, Elyra-AI
    * Model Development: TensorFlow, scikit-learn
    * Model Assessment: TensorBoard, AI toolkits
    * Model Deployment/ CI/CD: Kubeflow, KFServing/KNative, Sledon
    * Experiment Tracking: MLFlow


* Using the Storage Layer  
Description: This chapter explains how a modern data lake storage layer looks like. It introduces low level storage (Ceph for onprem, S3 of cloud), data mart for highly interactive queries (PostgreSQL) and data virtualization (Apache Iceberg/Teiid) 
  * Tooling decision matrix
  * Apache Iceberg
  * PostgreSQL
  * Ceph
  * Teiid


* Data Ingestion and Transformation  
Description: This chapter describes how to ingest data into the data lake. It covers standard tasks like getting data from a (non) relational data source into the data lake including incremental updates and versioning. It also explains on how to access the storage layer using standard SQL and how to ingest subsets of data into a faster storage provider (PostgreSQL) supporting interactive queries 
  * Tooling decision matrix
  * Building Data Marts with PostgreSQL
  * Designing ETL pipelines with Apache SparkSQL
  * ...

* Data Exploration  
Description: This chapter explains how data exploration can be done efficiently. It covers pandas as this is the de-facto standard for the task. But it also supports SQL as this is still used and understood by a majority of data scientists. Koalas supports the pandas API on SparkSQL. Besides slicing and icing, also data visualization is an incremental part of this task. This is why usage of seaboarn is introduced. Finally, BakerX promises to support the complete task of data exploration in a low code environment as jupyter plugin
  * Tooling decision matrix
  * Slicing and Dicing with Pandas
  * Slicing and Dicing on BigData with Koalas
  * Slicing and Dicing Apache SparkSQL
  * Data Exploration and Visualization with BakerX
  * Visualization with seaborn
  * ...

* Dashboarding  
Description: This chapter explains how reports / dashboards can be created as a deliverable to end users. In reality, this is where most of the current data science projects end. This is also a good starting point to discuss further automatization using machine learning
  * Tooling decision matrix
  * Enduser ready data products creation with Apache Superset
  * Report creation with BakerX, jupyter and seaborn
  * ...

* Model Development  
Description: This chapter explains how machine models should be built. It doesn’t introduce the frameworks used, but shows and exemplifies best practices on how those tools are used in an production context 
  * Tooling decision matrix
  * Hyperparameter Tuning with hyperopt and hparams
  * Parallel training on CPU clusters with TensorFlow
  * Parallel training on multiple GPUs, single node with TensorFlow
  * Parallel training on GPU clusters with TensorFlow
  * ...

* Model Assessment  
Description: Machine learning (and especially Deep Learning) models need to be proven to be robust before production deployment. This chapter explains how to accomplish these tasks in an automated way (CI/CD compatibility)
  * Tooling decision matrix
  * Neural Network Debugging with TensorBoard (jerome)
  * Bias Detection with AIF360
  * Model Explanation with AIX360
  * Adversarial Robustness with ART
  * ...

* Model Deployment / CI/CD  
Description: This chapter explains how to contineously integrate and deploy data products and machine learning models. It shows how reproducibility and transparency can be achieved. 
  * Tooling decision matrix
  * Model Serving with TFServing
  * Model Serving with Seldon
  * Model Serving with KNative and KFServing
  * Serving the Edge with TFLite
  * Serving the Web with TensorFlow.js
  * Model Monitoring
  * Building AI Model Libraries with MAX
  * ...


