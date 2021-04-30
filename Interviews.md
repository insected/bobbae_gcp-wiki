- [General](#general)
- [Coding](#coding)
  * [Shell](#shell)
    + [write a simple bash shell script](#write-a-simple-bash-shell-script)
    + [write a simple loop in bash shell](#write-a-simple-loop-in-bash-shell)
    + [how to handle command line argument limit restrictions](#how-to-handle-command-line-argument-limit-restrictions)
    + [what are file permissions bits (e.g. 0777), umask, ulimit](#what-are-file-permissions-bits--eg-0777---umask--ulimit)
      - [explain rwx vs 07](#explain-rwx-vs-07)
    + [what is fsck](#what-is-fsck)
    + [multiple processes, background vs. foreground](#multiple-processes--background-vs-foreground)
    + [terminal, termcap, tty, pty, screen, tmux](#terminal--termcap--tty--pty--screen--tmux)
    + [command line editing, key bindings, text editor, regexp](#command-line-editing--key-bindings--text-editor--regexp)
  * [python](#python)
  * [perl](#perl)
  * [java](#java)
  * [Awk](#awk)
  * [Programming in general](#programming-in-general)
    + [do you have any samples, github repo, open source projects?](#do-you-have-any-samples--github-repo--open-source-projects-)
    + [linked list](#linked-list)
    + [data structure](#data-structure)
    + [algorithm](#algorithm)
    + [Amazon, Microsoft coding Qs](#amazon--microsoft-coding-qs)
- [General Computer Science](#general-computer-science)
- [Google Cloud Platform](#google-cloud-platform)
- [General Infrastructure](#general-infrastructure)
  * [do you have and cloud certification ?   what kinds?](#do-you-have-and-cloud-certification-----what-kinds-)
  * [do you wish to study and pass certification tests?](#do-you-wish-to-study-and-pass-certification-tests-)
  * [have you applied and tested for certificates?  success or failures?](#have-you-applied-and-tested-for-certificates---success-or-failures-)
  * [virtualization](#virtualization)
  * [Hypervisors](#hypervisors)
  * [aws, azure, gcp](#aws--azure--gcp)
  * [docker](#docker)
  * [kubernetes](#kubernetes)
  * [General Compute  questions](#general-compute--questions)
    + [Describe what is big endian vs little endian](#describe-what-is-big-endian-vs-little-endian)
    + [Examples of CPUs that are big endian](#examples-of-cpus-that-are-big-endian)
    + [How can you tell whether a computer is big endian or not programmatically?](#how-can-you-tell-whether-a-computer-is-big-endian-or-not-programmatically-)
    + [Why does the endianness matter?](#why-does-the-endianness-matter-)
  * [why do modern computers use two's compliment representation](#why-do-modern-computers-use-two-s-compliment-representation)
  * [what is "Turing complete"](#what-is--turing-complete-)
  * [what is "Von Neumann" architecture](#what-is--von-neumann--architecture)
  * [RISC vs CISC](#risc-vs-cisc)
  * [example of RISC](#example-of-risc)
    + [Classic RISC  pipeline](#classic-risc--pipeline)
  * [Process vs threads](#process-vs-threads)
  * [thread vs coroutines](#thread-vs-coroutines)
  * [What are processor cores?](#what-are-processor-cores-)
  * [What is SIMD?](#what-is-simd-)
  * [OS questions](#os-questions)
  * [Linux](#linux)
  * [Linux, Unix](#linux--unix)
  * [RAM, cache, cache-line, registers, hard disk, flash disk, different parts of computer](#ram--cache--cache-line--registers--hard-disk--flash-disk--different-parts-of-computer)
- [general devops questions](#general-devops-questions)
  * [jenkins](#jenkins)
  * [jenkins , teamcity, bamboo, tavis, circle-ci, codeship](#jenkins---teamcity--bamboo--tavis--circle-ci--codeship)
  * [building docker images](#building-docker-images)
  * [VERY BASIC](#very-basic)
    + [Details of the CPU](#details-of-the-cpu)
    + [Details of the memory](#details-of-the-memory)
    + [Details of the storage](#details-of-the-storage)
    + [Details of the network](#details-of-the-network)
    + [How do these things matter when selecting a type of virtual machine in cloud compute services?](#how-do-these-things-matter-when-selecting-a-type-of-virtual-machine-in-cloud-compute-services-)
- [generic IT and sysadmin questions](#generic-it-and-sysadmin-questions)
  * [Windoes IT admin](#windoes-it-admin)
  * [kernel](#kernel)
  * [system call](#system-call)
  * [signals](#signals)
  * [filesystem](#filesystem)
  * [Bash, zsh, csh, ...](#bash--zsh--csh--)
- [Data Science](#data-science)
- [Data Engineering](#data-engineering)
  * [Composer & Apache Airflow questions](#composer---apache-airflow-questions)
    + [What is Cloud Composer?](#what-is-cloud-composer-)
    + [What is Apache Airflow?](#what-is-apache-airflow-)
    + [What are differences between airflow / composer and beam / dataflow?](#what-are-differences-between-airflow---composer-and-beam---dataflow-)
    + [How do I reuse code between DAG files?](#how-do-i-reuse-code-between-dag-files-)
    + [How do I minimize the risk of different definitions arising?](#how-do-i-minimize-the-risk-of-different-definitions-arising-)
    + [How do I set dependencies between DAGs?](#how-do-i-set-dependencies-between-dags-)
    + [How do I pass unique run IDs to a DAG and its tasks?](#how-do-i-pass-unique-run-ids-to-a-dag-and-its-tasks-)
    + [Where do I draw the line between tasks in a DAG?](#where-do-i-draw-the-line-between-tasks-in-a-dag-)
    + [Should I define multiple tasks in a single DAG to aggregate data from multiple sources?](#should-i-define-multiple-tasks-in-a-single-dag-to-aggregate-data-from-multiple-sources-)
    + [How do I limit the number of concurrent tasks running in a DAG?](#how-do-i-limit-the-number-of-concurrent-tasks-running-in-a-dag-)
  * [How is SQL Azure different than SQL server?](#how-is-sql-azure-different-than-sql-server-)
  * [How many replicas are maintained for each SQL Azure database?](#how-many-replicas-are-maintained-for-each-sql-azure-database-)
  * [How can we migrate from SQL server to SQL Azure?](#how-can-we-migrate-from-sql-server-to-sql-azure-)
  * [Which tools are available to manage SQL Azure databases and servers?](#which-tools-are-available-to-manage-sql-azure-databases-and-servers-)
  * [Tell me something about security and SQL Azure.](#tell-me-something-about-security-and-sql-azure)
  * [How do we synchronize On-Premise SQL server with SQL Azure?](#how-do-we-synchronize-on-premise-sql-server-with-sql-azure-)
  * [How do we Backup SQL Azure Data?](#how-do-we-backup-sql-azure-data-)
  * [What is the current limitation of the size of SQL Azure DB?](#what-is-the-current-limitation-of-the-size-of-sql-azure-db-)
  * [How do you handle datasets larger than 50 GB?](#how-do-you-handle-datasets-larger-than-50-gb-)
  * [What happens when the SQL Azure database reaches Max Size?](#what-happens-when-the-sql-azure-database-reaches-max-size-)
  * [How many databases can we create on a single server?](#how-many-databases-can-we-create-on-a-single-server-)
  * [What is Power BI?](#what-is-power-bi-)
  * [What data sources can Power BI connect to?](#what-data-sources-can-power-bi-connect-to-)
  * [What are Building Blocks in Power BI?](#what-are-building-blocks-in-power-bi-)
  * [What are the different types of filters in Power BI Reports?](#what-are-the-different-types-of-filters-in-power-bi-reports-)
  * [What is DAX?](#what-is-dax-)
  * [What are the most common DAX Functions used?](#what-are-the-most-common-dax-functions-used-)
  * [What is Power Query?](#what-is-power-query-)
  * [What are the data destinations for Power Queries?](#what-are-the-data-destinations-for-power-queries-)
  * [Can SQL and Power Query/Query Editor be used together?](#can-sql-and-power-query-query-editor-be-used-together-)
  * [What are the primary requirement for a table to be used in Power Map?](#what-are-the-primary-requirement-for-a-table-to-be-used-in-power-map-)
  * [Compare QlikView with Tableau](#compare-qlikview-with-tableau)
  * [What are Filters? How many types of Filters are there in Tableau?](#what-are-filters--how-many-types-of-filters-are-there-in-tableau-)
  * [How is the Context Filter different from other Filters?](#how-is-the-context-filter-different-from-other-filters-)
  * [What is the disadvantage of Context Filters?](#what-is-the-disadvantage-of-context-filters-)
  * [What are the five main products offered by Tableau?](#what-are-the-five-main-products-offered-by-tableau-)
  * [What is data visualization?](#what-is-data-visualization-)
  * [Why Tableau?](#why-tableau-)
  * [What is aggregation and disaggregation of data?](#what-is-aggregation-and-disaggregation-of-data-)
  * [How to combine two Excel files with the same fields but different data (different years)?](#how-to-combine-two-excel-files-with-the-same-fields-but-different-data--different-years--)
  * [What is the difference between joining and blending in Tableau?](#what-is-the-difference-between-joining-and-blending-in-tableau-)
  * [What are Dimensions and Facts?](#what-are-dimensions-and-facts-)
  * [What is the difference between heat map and treemap?](#what-is-the-difference-between-heat-map-and-treemap-)
  * [What is the different between twb and twbx file extensions. Please explain.](#what-is-the-different-between-twb-and-twbx-file-extensions-please-explain)
  * [What is the use of the new custom SQL query in Tableau?](#what-is-the-use-of-the-new-custom-sql-query-in-tableau-)
  * [What are the similarities and differences between Tableau and Palantir?](#what-are-the-similarities-and-differences-between-tableau-and-palantir-)
  * [How can we combine a database and the flat file data in Tableau Desktop?](#how-can-we-combine-a-database-and-the-flat-file-data-in-tableau-desktop-)
  * [What is data modeling?](#what-is-data-modeling-)
  * [Load CSV data into BigQuery via CLI](#load-csv-data-into-bigquery-via-cli)
  * [Load CSV data into BigQuery via Go](#load-csv-data-into-bigquery-via-go)
  * [Load CSV data into BigQuery in python](#load-csv-data-into-bigquery-in-python)
  * [How to stream insert data into BigQuery](#how-to-stream-insert-data-into-bigquery)
  * [How do query via CLI](#how-do-query-via-cli)
  * [How to query via Go:](#how-to-query-via-go-)
  * [How to query via python](#how-to-query-via-python)
  * [Query BigTable data from BigQuery](#query-bigtable-data-from-bigquery)
  * [Query Cloud Storage from BigQuery](#query-cloud-storage-from-bigquery)
  * [Query Google Drive data from BigQuery](#query-google-drive-data-from-bigquery)
  * [Dataflow & Apache Beam questions](#dataflow---apache-beam-questions)
    + [What is Apache Beam?](#what-is-apache-beam-)
    + [Why we actually need Apache beam when we already have Hadoop/Spark/Flink?](#why-we-actually-need-apache-beam-when-we-already-have-hadoop-spark-flink-)
    + [What is Apache Flink?](#what-is-apache-flink-)
    + [What is Apache Apex](#what-is-apache-apex)
    + [What are five main concepts in beam?](#what-are-five-main-concepts-in-beam-)
    + [Is it possible to share data across pipeline instances in Google Cloud dataflow?](#is-it-possible-to-share-data-across-pipeline-instances-in-google-cloud-dataflow-)
    + [In Cloud dataflow, is it possible to access my job's worker machines (Compute Engine VMs) while my pipeline is running?](#in-cloud-dataflow--is-it-possible-to-access-my-job-s-worker-machines--compute-engine-vms--while-my-pipeline-is-running-)
    + [In the Cloud Dataflow Monitoring Interface, why don't I see Reserved CPU Time for my streaming job?](#in-the-cloud-dataflow-monitoring-interface--why-don-t-i-see-reserved-cpu-time-for-my-streaming-job-)
    + [In the Cloud Dataflow Monitoring Interface, why are the job state and watermark information unavailable for recently updated streaming jobs?](#in-the-cloud-dataflow-monitoring-interface--why-are-the-job-state-and-watermark-information-unavailable-for-recently-updated-streaming-jobs-)
    + [Can I pass additional (out-of-band) data into an existing ParDo operation?](#can-i-pass-additional--out-of-band--data-into-an-existing-pardo-operation-)
  * [Data warehouses](#data-warehouses)
    + [What are differences between Operational database and Data warehouse?](#what-are-differences-between-operational-database-and-data-warehouse-)
    + [What is ETL vs ELT?](#what-is-etl-vs-elt-)
    + [what are differences between OLTP and OLAP?](#what-are-differences-between-oltp-and-olap-)
    + [What is Data Cube?](#what-is-data-cube-)
    + [What are some OLAP operations?](#what-are-some-olap-operations-)
    + [what are star and snowflake schemas?](#what-are-star-and-snowflake-schemas-)
    + [What is dimensional modeling?](#what-is-dimensional-modeling-)
    + [What are slowly changing dimensions in Data warehouse applications?](#what-are-slowly-changing-dimensions-in-data-warehouse-applications-)
    + [What are Materialized Views in BigQuery?](#what-are-materialized-views-in-bigquery-)
    + [What are some example sources of data that can be loaded into BigQuery?](#what-are-some-example-sources-of-data-that-can-be-loaded-into-bigquery-)
    + [What input data formats are supported in BigQuery?](#what-input-data-formats-are-supported-in-bigquery-)
    + [What is external data source in BigQuery?](#what-is-external-data-source-in-bigquery-)
  * [What is the command to initialize Gcloud SDK](#what-is-the-command-to-initialize-gcloud-sdk)
  * [What is the cli command to list gcloud configuration](#what-is-the-cli-command-to-list-gcloud-configuration)
  * [What is the cli command to view information about Cloud SDK installation and active SDK configuration?](#what-is-the-cli-command-to-view-information-about-cloud-sdk-installation-and-active-sdk-configuration-)
  * [How to get a list of compute instances?](#how-to-get-a-list-of-compute-instances-)
  * [What are zones vs regions?](#what-are-zones-vs-regions-)
  * [How to create a dataproc cluster?](#how-to-create-a-dataproc-cluster-)
  * [How to submit a job to dataproc cluster?](#how-to-submit-a-job-to-dataproc-cluster-)
  * [What are goroutines?  And how are they used?](#what-are-goroutines---and-how-are-they-used-)
  * [What are channels? How are they used?](#what-are-channels--how-are-they-used-)
  * [Explain Go Interfaces?](#explain-go-interfaces-)
  * [How do you copy a slice?](#how-do-you-copy-a-slice-)
  * [How do you copy a map?](#how-do-you-copy-a-map-)
  * [How do you copy an interface?](#how-do-you-copy-an-interface-)
  * [How do you compare two structs?](#how-do-you-compare-two-structs-)
  * [How do you compare two interfaces?](#how-do-you-compare-two-interfaces-)
  * [How do you compare byte slices?](#how-do-you-compare-byte-slices-)
  * [What is wrong with the following code snippet?](#what-is-wrong-with-the-following-code-snippet-)
  * [What might be wrong with the following small program?](#what-might-be-wrong-with-the-following-small-program-)
  * [What is the difference, if any, in the following two slice declarations, and which one is more preferable?](#what-is-the-difference--if-any--in-the-following-two-slice-declarations--and-which-one-is-more-preferable-)
  * [Do you need both GOPATH and GOROOT variables, and why?](#do-you-need-both-gopath-and-goroot-variables--and-why-)
  * [What is GraphQL?](#what-is-graphql-)
  * [List the key concepts of the GraphQL query language](#list-the-key-concepts-of-the-graphql-query-language)
  * [Explain the main difference between REST and GraphQL](#explain-the-main-difference-between-rest-and-graphql)
  * [How to do Server-side Caching? Or, what is a common challenge facing GraphQL.](#how-to-do-server-side-caching--or--what-is-a-common-challenge-facing-graphql)
  * [Are there any disadvantages to GraphQL?](#are-there-any-disadvantages-to-graphql-)
  * [what is GraphQL Schema?](#what-is-graphql-schema-)
  * [Is GraphQL a Database Technology?](#is-graphql-a-database-technology-)
  * [Hadoop questions](#hadoop-questions)
    + [What are some of the important features of Hadoop?](#what-are-some-of-the-important-features-of-hadoop-)
    + [How are files stored in Hadoop?  What are Blocks?  What is the size of a Block in Hadoop?](#how-are-files-stored-in-hadoop---what-are-blocks---what-is-the-size-of-a-block-in-hadoop-)
    + [What do Block Scanners  do in Hadoop?](#what-do-block-scanners--do-in-hadoop-)
    + [In Hadoop what are different Node types?](#in-hadoop-what-are-different-node-types-)
    + [What is a NameNode?  What does it do?](#what-is-a-namenode---what-does-it-do-)
    + [What may occur if NameNode crashes in the HDFS cluster?](#what-may-occur-if-namenode-crashes-in-the-hdfs-cluster-)
    + [Which are the two messages, which NameNode gets from DataNode within Hadoop?](#which-are-the-two-messages--which-namenode-gets-from-datanode-within-hadoop-)
    + [How does Indexing work when it comes to Hadoop.](#how-does-indexing-work-when-it-comes-to-hadoop)
    + [What are the types of configurations (or configuration files) when it comes to Hadoop?](#what-are-the-types-of-configurations--or-configuration-files--when-it-comes-to-hadoop-)
    + [How does inner-cluster data copying function work within Hadoop?](#how-does-inner-cluster-data-copying-function-work-within-hadoop-)
    + [What is Apache HBase?](#what-is-apache-hbase-)
    + [What is the reason of using HBase?](#what-is-the-reason-of-using-hbase-)
    + [Define the difference between hive and HBase?](#define-the-difference-between-hive-and-hbase-)
    + [Define column families?](#define-column-families-)
    + [What is decorating Filters?](#what-is-decorating-filters-)
    + [Define MapReduce.](#define-mapreduce)
    + [Illustrate a simple example of the working of MapReduce.](#illustrate-a-simple-example-of-the-working-of-mapreduce)
    + [What is Shuffling and Sorting in MapReduce?](#what-is-shuffling-and-sorting-in-mapreduce-)
    + [What is Partitioner and its usage?](#what-is-partitioner-and-its-usage-)
    + [What is Identity Mapper and Chain Mapper?](#what-is-identity-mapper-and-chain-mapper-)
    + [What are the key differences between Pig vs MapReduce?](#what-are-the-key-differences-between-pig-vs-mapreduce-)
    + [What is partitioning?](#what-is-partitioning-)
    + [What is Google Cloud Dataproc?](#what-is-google-cloud-dataproc-)
    + [What are the operational commands of HBase?](#what-are-the-operational-commands-of-hbase-)
    + [What is the use of ZooKeeper?](#what-is-the-use-of-zookeeper-)
    + [What is the  distributed consensus algorithm used in Zookeeper? What are alternatives?](#what-is-the--distributed-consensus-algorithm-used-in-zookeeper--what-are-alternatives-)
    + [Define compaction in HBase?](#define-compaction-in-hbase-)
    + [Compare HBase with Hive?](#compare-hbase-with-hive-)
    + [Compare HBase with Cassandra?](#compare-hbase-with-cassandra-)
    + [additional questions](#additional-questions)
  * [What is Kafka?](#what-is-kafka-)
  * [List the various components in Kafka.](#list-the-various-components-in-kafka)
  * [Explain the role of the offset.](#explain-the-role-of-the-offset)
  * [What is a Consumer Group?](#what-is-a-consumer-group-)
  * [What is the role of the ZooKeeper?](#what-is-the-role-of-the-zookeeper-)
  * [Is it possible to use Kafka without ZooKeeper?](#is-it-possible-to-use-kafka-without-zookeeper-)
  * [Explain the concept of Leader and Follower.](#explain-the-concept-of-leader-and-follower)
  * [What roles do Replicas and the ISR play?](#what-roles-do-replicas-and-the-isr-play-)
  * [Why are Replications critical in Kafka?](#why-are-replications-critical-in-kafka-)
  * [If a Replica stays out of the ISR for a long time, what does it signify?](#if-a-replica-stays-out-of-the-isr-for-a-long-time--what-does-it-signify-)
  * [What is the process for starting a Kafka server?](#what-is-the-process-for-starting-a-kafka-server-)
  * [How do you define a Partitioning Key?](#how-do-you-define-a-partitioning-key-)
  * [In the Producer, when does QueueFullException occur?](#in-the-producer--when-does-queuefullexception-occur-)
  * [Explain the role of the Kafka Producer API.](#explain-the-role-of-the-kafka-producer-api)
  * [What is the main difference between Kafka and Flume?](#what-is-the-main-difference-between-kafka-and-flume-)
  * [What are different types of ML?](#what-are-different-types-of-ml-)
  * [How does deep learning differ from ML?](#how-does-deep-learning-differ-from-ml-)
  * [Explain classification and regression](#explain-classification-and-regression)
  * [What is selection bias?](#what-is-selection-bias-)
  * [what is precision and recall?](#what-is-precision-and-recall-)
  * [what is confusion matrix?](#what-is-confusion-matrix-)
  * [What is the difference between inductive and deductive learning?](#what-is-the-difference-between-inductive-and-deductive-learning-)
  * [How is KNN different from K-means clustering?](#how-is-knn-different-from-k-means-clustering-)
  * [Is it better to have too many false positives or too many false negatives? Explain.](#is-it-better-to-have-too-many-false-positives-or-too-many-false-negatives--explain)
  * [What is the difference between Gini Impurity and Entropy in a Decision Tree?](#what-is-the-difference-between-gini-impurity-and-entropy-in-a-decision-tree-)
  * [What is the difference between Entropy and Information Gain?](#what-is-the-difference-between-entropy-and-information-gain-)
  * [What is Overfitting? And how do you ensure you’re not overfitting with a model?](#what-is-overfitting--and-how-do-you-ensure-you-re-not-overfitting-with-a-model-)
  * [How would you screen for outliers and what should you do if you find one?](#how-would-you-screen-for-outliers-and-what-should-you-do-if-you-find-one-)
  * [What is bagging and boosting in Machine Learning?](#what-is-bagging-and-boosting-in-machine-learning-)
  * [What are collinearity and multicollinearity?](#what-are-collinearity-and-multicollinearity-)
  * [What do you understand by Eigenvectors and Eigenvalues?](#what-do-you-understand-by-eigenvectors-and-eigenvalues-)
  * [What is A/B Testing?](#what-is-a-b-testing-)
  * [What is Cluster Sampling?](#what-is-cluster-sampling-)
  * [You are given a data set consisting of variables having more than 30% missing values? Let’s say, out of 50 variables, 8 variables have missing values higher than 30%. How will you deal with them?](#you-are-given-a-data-set-consisting-of-variables-having-more-than-30--missing-values--let-s-say--out-of-50-variables--8-variables-have-missing-values-higher-than-30--how-will-you-deal-with-them-)
  * [There’s a game where you are asked to roll two fair six-sided dice. If the sum of the values on the dice equals seven, then you win $21. However, you must pay $5 to play each time you roll both dice. Do you play this game? And in the follow-up: If he plays 6 times what is the probability of making money from this game?](#there-s-a-game-where-you-are-asked-to-roll-two-fair-six-sided-dice-if-the-sum-of-the-values-on-the-dice-equals-seven--then-you-win--21-however--you-must-pay--5-to-play-each-time-you-roll-both-dice-do-you-play-this-game--and-in-the-follow-up--if-he-plays-6-times-what-is-the-probability-of-making-money-from-this-game-)
  * [‘People who bought this also bought…’ recommendations seen on Amazon is based on which algorithm?](#-people-who-bought-this-also-bought---recommendations-seen-on-amazon-is-based-on-which-algorithm-)
  * [What is PCA?](#what-is-pca-)
  * [You are given a data set. The data set contains many variables, some of which are highly correlated and you know about it. Your manager has asked you to run PCA. Would you remove correlated variables first? Why?](#you-are-given-a-data-set-the-data-set-contains-many-variables--some-of-which-are-highly-correlated-and-you-know-about-it-your-manager-has-asked-you-to-run-pca-would-you-remove-correlated-variables-first--why-)
  * [What is Boosting?](#what-is-boosting-)
  * [What is Gradient Boosting in Machine Learning:](#what-is-gradient-boosting-in-machine-learning-)
  * [What’s an ensemble?](#what-s-an-ensemble-)
  * [Difference betweeen random frest and GBM?  "Averaging the predictions made by lots of predictors”.. that sounds like Random Forest!](#difference-betweeen-random-frest-and-gbm----averaging-the-predictions-made-by-lots-of-predictors--that-sounds-like-random-forest-)
  * [how does the algorithm decide the number of predictors to put in the ensemble?](#how-does-the-algorithm-decide-the-number-of-predictors-to-put-in-the-ensemble-)
  * [Finding the best set of hyperparameters](#finding-the-best-set-of-hyperparameters)
  * [Explain the working of decision trees and XGBoost and all the models(Bagging, Random Forest, Boosting, Gradient Boosting) in between. Talk about parallelization in these models. Talk about bias/variance for these models.](#explain-the-working-of-decision-trees-and-xgboost-and-all-the-models-bagging--random-forest--boosting--gradient-boosting--in-between-talk-about-parallelization-in-these-models-talk-about-bias-variance-for-these-models)
  * [Why does XGBoost perform so well?](#why-does-xgboost-perform-so-well-)
  * [So should we use just XGBoost all the time?](#so-should-we-use-just-xgboost-all-the-time-)
  * [Additional predictive modeling questions](#additional-predictive-modeling-questions)
  * [What is Tensorflow?](#what-is-tensorflow-)
  * [What are Tensors?](#what-are-tensors-)
  * [What is a TensorBoard?](#what-is-a-tensorboard-)
  * [List a few advantages of TensorFlow?](#list-a-few-advantages-of-tensorflow-)
  * [List a few limitations of Tensorflow.](#list-a-few-limitations-of-tensorflow)
  * [What are TensorFlow servables?](#what-are-tensorflow-servables-)
  * [What do the TensorFlow managers do?](#what-do-the-tensorflow-managers-do-)
  * [What are TensorFlow loaders?](#what-are-tensorflow-loaders-)
  * [What do you mean by sources in TensorFlow?](#what-do-you-mean-by-sources-in-tensorflow-)
  * [What are the APIs inside the TensorFlow project?](#what-are-the-apis-inside-the-tensorflow-project-)
  * [What are the APIs outside TensorFlow project?](#what-are-the-apis-outside-tensorflow-project-)
  * [In TensorFlow, what exactly Bias and Variance are? Do you find any similarity between them?](#in-tensorflow--what-exactly-bias-and-variance-are--do-you-find-any-similarity-between-them-)
  * [Can TensorFlow be deployed in container software?](#can-tensorflow-be-deployed-in-container-software-)
  * [What exactly Neural Networks are? What are the types of same you are familiar with?](#what-exactly-neural-networks-are--what-are-the-types-of-same-you-are-familiar-with-)
  * [What are the general advantages of using the Artifical Neural Networks?](#what-are-the-general-advantages-of-using-the-artifical-neural-networks-)
  * [What exactly do you know about Recall and Precision?](#what-exactly-do-you-know-about-recall-and-precision-)
  * [What difference do you find in Type I and Type II errors?](#what-difference-do-you-find-in-type-i-and-type-ii-errors-)
  * [What would be your strategy to handle a situation indicating an imbalanced dataset?](#what-would-be-your-strategy-to-handle-a-situation-indicating-an-imbalanced-dataset-)
  * [What exactly do you know about Bias-Variance decomposition?](#what-exactly-do-you-know-about-bias-variance-decomposition-)
  * [What are word embeddings used for and can they be used in TensorFlow?](#what-are-word-embeddings-used-for-and-can-they-be-used-in-tensorflow-)
  * [What is the MNIST dataset?](#what-is-the-mnist-dataset-)
  * [What are Bayesian Statistics and Bayes Theorem?](#what-are-bayesian-statistics-and-bayes-theorem-)
  * [How is Bayesian useful in ML?  Or is ML different than Bayesian statistics?](#how-is-bayesian-useful-in-ml---or-is-ml-different-than-bayesian-statistics-)
    + [What are three naive Bayes classifiers?](#what-are-three-naive-bayes-classifiers-)
  * [What is MQTT in IoT?](#what-is-mqtt-in-iot-)
  * [Who uses MQTT?](#who-uses-mqtt-)
  * [How does MQTT work?](#how-does-mqtt-work-)
  * [What is an MQTT client?](#what-is-an-mqtt-client-)
  * [What does an MQTT broker do?](#what-does-an-mqtt-broker-do-)
  * [What is an MQTT topic?](#what-is-an-mqtt-topic-)
  * [Is MQTT secure?](#is-mqtt-secure-)
  * [Is MQTT open source?](#is-mqtt-open-source-)
  * [What is the difference between HTTP and MQTT?](#what-is-the-difference-between-http-and-mqtt-)
  * [What is the difference between AMQP and MQTT?](#what-is-the-difference-between-amqp-and-mqtt-)
  * [MQTT is a binary protocol with strength in simplicity to be ideal for mobile IoT app and M2M. It provides the pub/sub messaging pattern and is designed for resource-constrained devices, low bandwidth and high latency networks. MQTT is specified by the official OASIS Standard.](#mqtt-is-a-binary-protocol-with-strength-in-simplicity-to-be-ideal-for-mobile-iot-app-and-m2m-it-provides-the-pub-sub-messaging-pattern-and-is-designed-for-resource-constrained-devices--low-bandwidth-and-high-latency-networks-mqtt-is-specified-by-the-official-oasis-standard)
  * [Does MQTT use WebSockets?](#does-mqtt-use-websockets-)
  * [Does MQTT use TCP or UDP?](#does-mqtt-use-tcp-or-udp-)
  * [Does MQTT require internet?](#does-mqtt-require-internet-)
  * [Does MQTT work with Apache Kafka?](#does-mqtt-work-with-apache-kafka-)
  * [Is MQTT restful?](#is-mqtt-restful-)
  * [What are some NoSQL databases?  Please list and describe them](#what-are-some-nosql-databases---please-list-and-describe-them)
  * [What are some types of NoSQL databases?](#what-are-some-types-of-nosql-databases-)
  * [Can you describe which NoSQL database is which type?](#can-you-describe-which-nosql-database-is-which-type-)
  * [What are some NoSQL database features?](#what-are-some-nosql-database-features-)
  * [Give the name of some components of Cassandra and explain each.](#give-the-name-of-some-components-of-cassandra-and-explain-each)
  * [Tell something about the query language used in Cassandra Database.](#tell-something-about-the-query-language-used-in-cassandra-database)
  * [Define commit log.](#define-commit-log)
  * [Name the types of tunable consistency.](#name-the-types-of-tunable-consistency)
  * [Define SSTable.](#define-sstable)
  * [Describe Memtable.](#describe-memtable)
  * [Give a list of Collection data type in Cassandra.](#give-a-list-of-collection-data-type-in-cassandra)
  * [What is MongoDB?](#what-is-mongodb-)
  * [What do you understand by NoSQL databases? Is MongoDB a NoSQL database? Explain.](#what-do-you-understand-by-nosql-databases--is-mongodb-a-nosql-database--explain)
  * [What is the difference between MongoDB and MySQL?](#what-is-the-difference-between-mongodb-and-mysql-)
  * [What are mongoDB features?](#what-are-mongodb-features-)
  * [When and to what extent does data get extended to multi-slice?](#when-and-to-what-extent-does-data-get-extended-to-multi-slice-)
  * [Compare MongoDB with Couchbase and CouchbaseDB.](#compare-mongodb-with-couchbase-and-couchbasedb)
  * [When do we use a namespace in MongoDB?](#when-do-we-use-a-namespace-in-mongodb-)
  * [If you remove an object attribute, is it deleted from the database?](#if-you-remove-an-object-attribute--is-it-deleted-from-the-database-)
  * [How can we move an old file into the moveChunk directory?](#how-can-we-move-an-old-file-into-the-movechunk-directory-)
  * [Explain the situation when an index does not fit into RAM.](#explain-the-situation-when-an-index-does-not-fit-into-ram)
  * [How does MongoDB provide consistency?](#how-does-mongodb-provide-consistency-)
  * [Why is MongoDB not chosen for a 32-bit system?](#why-is-mongodb-not-chosen-for-a-32-bit-system-)
  * [How does Journaling work in MongoDB?](#how-does-journaling-work-in-mongodb-)
  * [How can you isolate the cursors from intervening with the write operations?](#how-can-you-isolate-the-cursors-from-intervening-with-the-write-operations-)
  * [what is CRUD?](#what-is-crud-)
  * [Explain Replication.](#explain-replication)
  * [What is the use of GridFS in MongoDB?](#what-is-the-use-of-gridfs-in-mongodb-)
  * [Which command is used for inserting a document in MongoDB?](#which-command-is-used-for-inserting-a-document-in-mongodb-)
  * [What type of data is stored by MongoDB?](#what-type-of-data-is-stored-by-mongodb-)
  * [Define Horizontal Scaling.](#define-horizontal-scaling)
  * [Define the Aggregation pipeline.](#define-the-aggregation-pipeline)
  * [Define MapReduce.](#define-mapreduce-1)
  * [Pandas questions](#pandas-questions)
    + [What are important data structures in pandas?](#what-are-important-data-structures-in-pandas-)
    + [what are Series in Pandas?](#what-are-series-in-pandas-)
    + [What Is A pandas DataFrame? How Will You Create An Empty DataFrame In pandas?](#what-is-a-pandas-dataframe--how-will-you-create-an-empty-dataframe-in-pandas-)
    + [How do you Create a DataFrame using List?](#how-do-you-create-a-dataframe-using-list-)
    + [How will you add a column to a pandas DataFrame?](#how-will-you-add-a-column-to-a-pandas-dataframe-)
    + [How to Delete Indices, Rows or Columns From a Pandas Data Frame?](#how-to-delete-indices--rows-or-columns-from-a-pandas-data-frame-)
    + [How to get the items of series A not present in series B?](#how-to-get-the-items-of-series-a-not-present-in-series-b-)
    + [How to get the items not common to both series A and series B?](#how-to-get-the-items-not-common-to-both-series-a-and-series-b-)
    + [How to get the minimum, 25th percentile, median, 75th, and max of a numeric series?](#how-to-get-the-minimum--25th-percentile--median--75th--and-max-of-a-numeric-series-)
    + [How to convert a numpy array to a dataframe of given shape?](#how-to-convert-a-numpy-array-to-a-dataframe-of-given-shape-)
  * [Python related data engineering questions](#python-related-data-engineering-questions)
    + [What Native Data Structures Can You Name in Python?](#what-native-data-structures-can-you-name-in-python-)
    + [In a List and in a Dictionary, What Are the Typical Characteristics of Elements?](#in-a-list-and-in-a-dictionary--what-are-the-typical-characteristics-of-elements-)
    + [Is There a Way to Get a List of All the Keys in a Dictionary? If So, How Would You Do It?](#is-there-a-way-to-get-a-list-of-all-the-keys-in-a-dictionary--if-so--how-would-you-do-it-)
    + [When Would You Use a List vs. a Tuple vs. a Set in Python?](#when-would-you-use-a-list-vs-a-tuple-vs-a-set-in-python-)
    + [Compare BeautifulSoup and Scrapy](#compare-beautifulsoup-and-scrapy)
    + [Name a few libraries in python used for Data analysis and scientific computations](#name-a-few-libraries-in-python-used-for-data-analysis-and-scientific-computations)
    + [Which library would you prefer for plotting in Python language: Seaborn or Matplotlib or Bokeh?](#which-library-would-you-prefer-for-plotting-in-python-language--seaborn-or-matplotlib-or-bokeh-)
    + [How are NumPy and SciPy related?](#how-are-numpy-and-scipy-related-)
    + [How can you handle duplicate values in a dataset for a variable in Python?](#how-can-you-handle-duplicate-values-in-a-dataset-for-a-variable-in-python-)
    + [Write a basic Machine Learning program to check the accuracy of a model,  by importing any dataset using any classifier?](#write-a-basic-machine-learning-program-to-check-the-accuracy-of-a-model---by-importing-any-dataset-using-any-classifier-)
  * [Spark questions](#spark-questions)
    + [What does a Spark Engine do?](#what-does-a-spark-engine-do-)
    + [What is RDD.](#what-is-rdd)
  * [Why is RDD immutable in Spark?](#why-is-rdd-immutable-in-spark-)
    + [What operations does an RDD support?](#what-operations-does-an-rdd-support-)
    + [What is the difference in cache() and persist() methods in Apache Spark?](#what-is-the-difference-in-cache---and-persist---methods-in-apache-spark-)
    + [What the functions of Spark Core.](#what-the-functions-of-spark-core)
    + [Does spark support data replication in memory?](#does-spark-support-data-replication-in-memory-)
    + [What is RDD Lineage?](#what-is-rdd-lineage-)
    + [What is Spark Driver?](#what-is-spark-driver-)
    + [What is Hive on Spark?](#what-is-hive-on-spark-)
    + [Name the commonly used Spark Ecosystems.](#name-the-commonly-used-spark-ecosystems)
    + [What is Spark Streaming.](#what-is-spark-streaming)
    + [What is a Parquet file?](#what-is-a-parquet-file-)
    + [What file systems does Apache Spark support?](#what-file-systems-does-apache-spark-support-)
    + [What is YARN?](#what-is-yarn-)
    + [List the functions of Spark SQL.](#list-the-functions-of-spark-sql)
    + [What are the benefits of Spark over MapReduce?](#what-are-the-benefits-of-spark-over-mapreduce-)
    + [Is there any benefit of learning MapReduce?](#is-there-any-benefit-of-learning-mapreduce-)
    + [What is Spark Executor?](#what-is-spark-executor-)
    + [Name the types of Cluster Managers in Spark.](#name-the-types-of-cluster-managers-in-spark)
    + [What is PageRank?](#what-is-pagerank-)
    + [Do you need to install Spark on all the nodes of the YARN cluster while running Spark on YARN?](#do-you-need-to-install-spark-on-all-the-nodes-of-the-yarn-cluster-while-running-spark-on-yarn-)
    + [Illustrate some demerits of using Spark.](#illustrate-some-demerits-of-using-spark)
    + [How to create an RDD?](#how-to-create-an-rdd-)
    + [additional questions](#additional-questions-1)
  * [SQL questions](#sql-questions)
    + [what are different kinds of statements in SQL?](#what-are-different-kinds-of-statements-in-sql-)
    + [What is a Primary Key? Can there be more than one Primary key?](#what-is-a-primary-key--can-there-be-more-than-one-primary-key-)
    + [What is a Foreign Key?](#what-is-a-foreign-key-)
    + [What is a Join? List its different types.](#what-is-a-join--list-its-different-types)
    + [What is a Self-Join?](#what-is-a-self-join-)
    + [What is a Cross-Join?](#what-is-a-cross-join-)
    + [What is the difference between Clustered and Non-clustered index?](#what-is-the-difference-between-clustered-and-non-clustered-index-)
    + [What are some common clauses used with SELECT query in SQL?](#what-are-some-common-clauses-used-with-select-query-in-sql-)
    + [What are UNION, MINUS and INTERSECT commands?](#what-are-union--minus-and-intersect-commands-)
    + [What is Cursor? How to use a Cursor?](#what-is-cursor--how-to-use-a-cursor-)
    + [What are Entities and Relationships?](#what-are-entities-and-relationships-)
    + [List the different types of relationships in SQL.](#list-the-different-types-of-relationships-in-sql)
    + [What is a View?](#what-is-a-view-)
    + [What is Normalization?](#what-is-normalization-)
    + [What is Denormalization?](#what-is-denormalization-)
    + [What are the TRUNCATE, DELETE and DROP statements?](#what-are-the-truncate--delete-and-drop-statements-)
    + [What is the difference between DROP and TRUNCATE statements?](#what-is-the-difference-between-drop-and-truncate-statements-)
    + [What is the difference between DELETE and TRUNCATE statements?](#what-is-the-difference-between-delete-and-truncate-statements-)
    + [What are Aggregate and Scalar functions?](#what-are-aggregate-and-scalar-functions-)
    + [What are transactions and its controls?](#what-are-transactions-and-its-controls-)
    + [What are 4 kinds of relations.](#what-are-4-kinds-of-relations)
    + [What is User-defined function? What are its various types?](#what-is-user-defined-function--what-are-its-various-types-)
    + [What is OLTP?](#what-is-oltp-)
    + [What are the differences between OLTP and OLAP?](#what-are-the-differences-between-oltp-and-olap-)
    + [What is Collation? What are the different types of Collation Sensitivity?](#what-is-collation--what-are-the-different-types-of-collation-sensitivity-)
    + [What is a Stored Procedure?](#what-is-a-stored-procedure-)
    + [What is Pattern Matching in SQL?](#what-is-pattern-matching-in-sql-)
    + [Write an SQL query that makes recommendations using the pages that your friends liked. Assume you have two tables: a two-column table of users and their friends, and a two-column table of users and the pages they liked. It should not recommend pages you already like.](#write-an-sql-query-that-makes-recommendations-using-the-pages-that-your-friends-liked-assume-you-have-two-tables--a-two-column-table-of-users-and-their-friends--and-a-two-column-table-of-users-and-the-pages-they-liked-it-should-not-recommend-pages-you-already-like)
    + [Find the month-over-month percentage change for monthly active users (MAU).](#find-the-month-over-month-percentage-change-for-monthly-active-users--mau-)
    + [Write SQL such that each node can be left, inner, or Root node, for input table that has node number and parent node id.](#write-sql-such-that-each-node-can-be-left--inner--or-root-node--for-input-table-that-has-node-number-and-parent-node-id)
- [data engineering verbal questions](#data-engineering-verbal-questions)
  * [General questions and strategy](#general-questions-and-strategy)
    + [What is data engineering?](#what-is-data-engineering-)
    + [What are the most important languages/skills you’ve learned and use on a daily basis?](#what-are-the-most-important-languages-skills-you-ve-learned-and-use-on-a-daily-basis-)
    + [Describe some of the projects from your current role. How do you think you’ll be able to apply your experience there with our company?](#describe-some-of-the-projects-from-your-current-role-how-do-you-think-you-ll-be-able-to-apply-your-experience-there-with-our-company-)
    + [What are some of the most common problems you’ve run into with your work? What’s the biggest problem you’ve ever run into? How did you overcome these challenges?](#what-are-some-of-the-most-common-problems-you-ve-run-into-with-your-work--what-s-the-biggest-problem-you-ve-ever-run-into--how-did-you-overcome-these-challenges-)
    + [Can you describe a time where you found a new use case for an existing database?](#can-you-describe-a-time-where-you-found-a-new-use-case-for-an-existing-database-)
    + [What Is the Biggest Challenge Facing Your Current Job Right Now? What Is Your Biggest Failure?](#what-is-the-biggest-challenge-facing-your-current-job-right-now--what-is-your-biggest-failure-)
    + [What Is the Accomplishment You Are Most Proud Of?](#what-is-the-accomplishment-you-are-most-proud-of-)
    + [What are some of your favorite programming languages and frameworks? Do you have a github or gitlab URL?](#what-are-some-of-your-favorite-programming-languages-and-frameworks--do-you-have-a-github-or-gitlab-url-)
    + [What is CAP theorem in the context of distributed databases ?](#what-is-cap-theorem-in-the-context-of-distributed-databases--)
    + [Why can a system not have all three properties of the CAP theorem?](#why-can-a-system-not-have-all-three-properties-of-the-cap-theorem-)
    + [What is ACID in the context of databases?](#what-is-acid-in-the-context-of-databases-)
    + [what does BASE mean in database as opposed to ACID in the context of databases?](#what-does-base-mean-in-database-as-opposed-to-acid-in-the-context-of-databases-)
    + [what is Cloud SQL?](#what-is-cloud-sql-)
    + [what is Cloud Bigtable?](#what-is-cloud-bigtable-)
    + [what is Cloud Spanner?](#what-is-cloud-spanner-)
    + [what is Cloud Memorystore?](#what-is-cloud-memorystore-)
    + [what is Cloud Firestore?](#what-is-cloud-firestore-)
    + [what is Firebase Realtime Database?](#what-is-firebase-realtime-database-)
    + [what is BigQuery?](#what-is-bigquery-)
- [Cloud](#cloud)
  * [general cloud related questions](#general-cloud-related-questions)
- [Frontend](#frontend)
- [Backend](#backend)
- [Networking](#networking)
  * [General networking questions](#general-networking-questions)
  * [TCP/IP](#tcp-ip)
  * [Explain what happens when you ping 127.0.0.1](#explain-what-happens-when-you-ping-127001)
  * [Explain detailed steps of what happens when you google something](#explain-detailed-steps-of-what-happens-when-you-google-something)
- [network byte order](#network-byte-order)
- [Routing & switching](#routing---switching)
  * [IPv4 vs. IPv6](#ipv4-vs-ipv6)
  * [DNS](#dns)
  * [DHCP](#dhcp)
  * [VPN](#vpn)
  * [VLAN & VxLAN](#vlan---vxlan)
- [firewall](#firewall)
- [ssh](#ssh)
- [security, cryptography](#security--cryptography)
  * [IPSec](#ipsec)
  * [OpenVPN](#openvpn)
  * [Compare PPTP, IPSec, OpenVPN, wireguard](#compare-pptp--ipsec--openvpn--wireguard)
  * [Crypto agility](#crypto-agility)
  * [types of linux net devices](#types-of-linux-net-devices)
  * [OVN & OVS](#ovn---ovs)
- [IPv4 and IPv6](#ipv4-and-ipv6)
- [Storage](#storage)
  * [storage general](#storage-general)
  * [cloud storage](#cloud-storage)
    + [What is it?](#what-is-it-)
    + [buckets vs objects](#buckets-vs-objects)
    + [when is HMAC key useful](#when-is-hmac-key-useful)
    + [EBS](#ebs)
  * [persistent disk (GCP)](#persistent-disk--gcp-)
  * [nfs](#nfs)
  * [s3](#s3)
  * [RAID](#raid)
  * [LVM](#lvm)
  * [ceph](#ceph)
  * [ext2, 3, 4, xfs, btrfs, zfs, ...](#ext2--3--4--xfs--btrfs--zfs--)
  * [iSCSI](#iscsi)
  * [netapp](#netapp)
  * [SAN](#san)
  * [CIFS, smb](#cifs--smb)
  * [object storage vs. key value](#object-storage-vs-key-value)
  * [linux file systems](#linux-file-systems)
  * [Types of Google cloud storage services](#types-of-google-cloud-storage-services)
- [Hardware](#hardware)
- [Desktop Support](#desktop-support)
- [Statistics](#statistics)
- [Math](#math)
- [Bioinformatics](#bioinformatics)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

# General

https://www.qfles.com/interview-question/

https://www.wisdomjobs.com/e-university/all-skillsets-interview-questions.html

https://en.wikipedia.org/wiki/Cognitive_reflection_test

# Coding

https://leetcode.com/problemset/all/

https://hackr.io/blog/programming-interview-questions

https://www.interviewbit.com/coding-interview-questions/

https://www.educative.io/blog/google-coding-interview-questions

## Shell 

https://www.javatpoint.com/shell-scripting-interview-questions

### write a simple bash shell script

Execute a command.  If it ran successfully, print success. Otherwise print fail.

### write a simple loop in bash shell

print numeric values from 1 to 10

### how to handle command line argument limit restrictions

### what are file permissions bits (e.g. 0777), umask, ulimit

#### explain rwx vs 07

### what is fsck


### multiple processes, background vs. foreground

### terminal, termcap, tty, pty, screen, tmux

### command line editing, key bindings, text editor, regexp



## python

https://www.interviewbit.com/python-interview-questions/


## perl

https://www.tutorialspoint.com/perl/perl_interview_questions.htm

## java

https://www.journaldev.com/370/java-programming-interview-questions

## Awk

https://techgoeasy.com/unix-awk-command/






## Programming in general

https://www.indeed.com/hire/interview-questions/programmer


### do you have any samples, github repo, open source projects?

Describe the project.
Which languages used?
What frameworks.
Why?

### linked list

https://www.javatpoint.com/linked-list-interview-questions

### data structure

https://www.geeksforgeeks.org/commonly-asked-data-structure-interview-questions-set-1/

### algorithm

https://www.geeksforgeeks.org/top-10-algorithms-in-interview-questions/

### Amazon, Microsoft coding Qs

https://www.geeksforgeeks.org/must-do-coding-questions-for-companies-like-amazon-microsoft-adobe/





# General Computer Science

https://www.geeksforgeeks.org/most-asked-computer-science-subjects-interview-questions-in-amazon-microsoft-flipkart/amp/

https://www.guru99.com/computer-science-interview-questions.html

# Google Cloud Platform

https://www.qfles.com/interview-question/google-cloud-platform-interview-questions

# General Infrastructure






## do you have and cloud certification ?   what kinds?

Discuss details

## do you wish to study and pass certification tests?

What kind of certificates are you interested in?
Why?

## have you applied and tested for certificates?  success or failures?
```
AWS, Azure, GCP?

How did you prepare?

Cloud academy?
Cloud guru?
Linux Academy?
Coursera?
Udemy?
etc.?
```





## virtualization

https://www.unixarena.com/2019/08/virtualization-hypervisor-basic-interview-questions.html/

https://www.javatpoint.com/virtualization-in-cloud-computing

## Hypervisors

Types of hypervisors.

https://vapour-apps.com/what-is-hypervisor/

## aws, azure, gcp

https://www.javatpoint.com/aws-vs-azure-vs-google-cloud-platform

## docker

https://www.edureka.co/blog/interview-questions/docker-interview-questions/

## kubernetes

https://www.edureka.co/blog/interview-questions/kubernetes-interview-questions/

## General Compute  questions

### Describe what is big endian vs little endian

### Examples of CPUs that are big endian

### How can you tell whether a computer is big endian or not programmatically?

```
#include <stdio.h> 

/* function to show bytes in memory, from location start to start+n*/
void show_mem_rep(char *start, int n) 
{ 
	int i; 
	for (i = 0; i < n; i++) 
		printf(" %.2x", start[i]); 
	printf("\n"); 
} 

/*Main function to call above function for 0x01234567*/
int main() 
{ 
int i = 0x01234567; 
show_mem_rep((char *)&i, sizeof(i)); 
//getchar(); 
return 0; 
} 
```

If this prints `67 45 23 01` then little endian.  If you get `01 23 45 67` then big endian.

### Why does the endianness matter?
What happens when you write a binary file on big endian machine and
read it back in little endian machine?

what happens when you write non-binary data, e.g. ASCII, or UTF-8 data, into the files and read them back on different endian machines, does it matter much?

What needs to be done for binary data in the IP header read from network?

## why do modern computers use two's compliment representation

https://en.wikipedia.org/wiki/Two%27s_complement

https://stackoverflow.com/questions/1125304/why-prefer-twos-complement-over-sign-and-magnitude-for-signed-numbers

## what is "Turing complete"

https://en.wikipedia.org/wiki/Turing_completeness


## what is "Von Neumann" architecture

https://www.thecrazyprogrammer.com/2019/02/difference-between-von-neumann-and-harvard-architecture.html

## RISC vs CISC
https://www.microcontrollertips.com/risc-vs-cisc-architectures-one-better/

## example of RISC

https://binaryterms.com/risc-processor.html

### Classic RISC  pipeline

Why?

https://en.wikipedia.org/wiki/Classic_RISC_pipeline

## Process vs threads

https://www.tutorialspoint.com/difference-between-process-and-thread

## thread vs coroutines

https://stackoverflow.com/questions/1934715/difference-between-a-coroutine-and-a-thread

## What are processor cores?  

https://quizizz.com/admin/quiz/5ab28f10ba09bf0019b2b33a/cpu-cores

## What is SIMD?
http://ftp.cvut.cz/kernel/people/geoff/cell/ps3-linux-docs/CellProgrammingTutorial/BasicsOfSIMDProgramming.html



## OS questions

https://www.javatpoint.com/operating-system-interview-questions


## Linux

https://www.javatpoint.com/linux-interview-questions

## Linux, Unix

https://www.educba.com/linux-system-administration-interview-questions/

https://www.educba.com/linux-system-administration-interview-questions/

https://www.softwaretestinghelp.com/unix-vs-linux/



https://www.whizlabs.com/blog/top-linux-interview-questions-answers/

https://www.globalguideline.com/interview_questions/Questions.php?sc=Linux_OS_Management



https://www.guru99.com/unix-interview-questions.html

## RAM, cache, cache-line, registers, hard disk, flash disk, different parts of computer

https://medium.com/software-design/why-software-developers-should-care-about-cpu-caches-8da04355bb8a

# general devops questions

https://www.edureka.co/blog/interview-questions/top-devops-interview-questions-2016/


## jenkins

https://www.guru99.com/jenkins-interview-questions.html

## jenkins , teamcity, bamboo, tavis, circle-ci, codeship 

https://www.altexsoft.com/blog/engineering/comparison-of-most-popular-continuous-integration-tools-jenkins-teamcity-bamboo-travis-ci-and-more/

## building docker images

https://www.taniarascia.com/continuous-integration-pipeline-docker/

Explain what each line does in the following dockerfile

```
# Pull from a base image
FROM node:12-alpine

# Copy the files from the current directory to app/
COPY . app/

# Use app/ as the working directory
WORKDIR app/

# Install dependencies (npm ci is similar to npm i, but for automated builds)
RUN npm ci --only-production

# Build production client side React application
RUN npm run build

# Listen on the specified port
EXPOSE 5000

# Set Node server
ENTRYPOINT npm run start
```

## VERY BASIC

Regarding your own computer in  front of you, can you look up information on what hardware you have.
CPU, memory, storage, networking details as reported by your operating system (windows, macosx, linux, ...)
How did you look the information up?
What do they say?
Discuss details on each: cpu, memory, storage, network...

### Details of the CPU

### Details of the memory

### Details of the storage

### Details of the network

### How do these things matter when selecting a type of virtual machine in cloud compute services?

# generic IT and sysadmin questions

https://opensource.com/article/19/7/sysadmin-job-interview-questions

https://www.thebalancecareers.com/information-technology-it-job-interview-questions-2061206

https://www.wgu.edu/blog/common-it-job-interview-questions1911.html





## Windoes IT admin

https://www.cosmicnovo.com/2016/12/07/system-administrator-microsoft-interview/





## kernel

https://www.sanfoundry.com/linux-kernel-interview-questions/

## system call
https://www.globalguideline.com/interview_questions/Questions.php?sc=Unix_System_Calls


## signals

https://www.globalguideline.com/interview_questions/Questions.php?sc=Signal_Handling

## filesystem

https://narva.webgarden.com/menu/linux-interviw-questions/filesystem-management-1



## Bash, zsh, csh, ...
https://www.howtogeek.com/68563/htg-explains-what-are-the-differences-between-linux-shells/






# Data Science

https://towardsdatascience.com/top-30-data-science-interview-questions-7dd9a96d3f5c

https://ds-interviews.org/


https://github.com/bobbae/gcp/wiki/Data-Science

# Data Engineering

https://www.guru99.com/data-engineer-interview-questions.html

https://365datascience.com/career-advice/job-interview-tips/data-engineer-interview-questions/

https://realpython.com/data-engineer-interview-questions-python/

https://github.com/bobbae/gcp/wiki/Data-Engineering


## Composer & Apache Airflow questions

### What is Cloud Composer?
Cloud Composer is a fully managed workflow orchestration service that empowers you to author, schedule, and monitor pipelines that span across clouds and on-premises data centers. Built on the popular Apache Airflow open source project and operated using the Python programming language, Cloud Composer is free from lock-in and easy to use.

### What is Apache Airflow?
Apache Airflow is an open source tool used to programatically author, schedule, and monitor workflows. There are a few key terms to remember relating to Airflow that you'll see throughout the lab:

* DAG - a DAG (Directed Acyclic Graph) is a collection of organized tasks that you want to schedule and run. DAGs, also called workflows, are defined in standard Python files
* Operator - an Operator describes a single task in a workflow

### What are differences between airflow / composer and beam / dataflow?

Airflow: A platform to programmaticaly author, schedule and monitor data pipelines, by Airbnb. Use Airflow to author workflows as directed acyclic graphs (DAGs) of tasks. The Airflow scheduler executes your tasks on an array of workers while following the specified dependencies. Rich command lines utilities makes performing complex surgeries on DAGs a snap. The rich user interface makes it easy to visualize pipelines running in production, monitor progress and troubleshoot issues when needed; Apache Beam: A unified programming model. It implements batch and streaming data processing jobs that run on any execution engine. It executes pipelines on multiple execution environments.

Airflow can do anything. It has BashOperator and PythonOperator which means it can run any bash script or any Python script.
It is a way to organize (setup complicated data pipeline DAGs), schedule, monitor, trigger re-runs of data pipelines, in a easy-to-view and use UI.
Also, it is easy to setup and everything is in familiar Python code.
Doing pipelines in an organized manner (i.e using Airflow) means you don't waste time debugging a mess of data processing (cron) scripts all over the place.

Apache Beam is a wrapper for the many data processing frameworks (Spark, Flink etc.) out there.
The intent is so you just learn Beam and can run on multiple backends (Beam runners).
If you are familiar with Keras and TensorFlow/Theano/Torch, the relationship between Keras and its backends is similar to the relationship between Beam and its data processing backends.

Google Cloud Platform's Cloud Dataflow is one backend for running Beam on.
They call it the Dataflow runner.

GCP's offering, Cloud Composer, is a managed Airflow implementation as a service, running in a Kubernetes cluster in Google Kubernetes Engine (GKE).
So you can either:
- manual Airflow implementation, doing data processing on the instance itself (if your data is small (or your instance is powerful enough), you can process data on the machine running Airflow. This is why many are confused if Airflow can process data or not)
- manual Airflow implementation calling Beam jobs
- Cloud Composer (managed Airflow as a service) calling jobs in Cloud Dataflow
- Cloud Composer running data processing containers in Composer's Kubernetes cluster environment itself, using Airflow's KubernetesPodOperator (KPO)
- Cloud Composer running data processing containers in Composer's Kubernetes cluster environment with Airflow's KPO, but this time in a better isolated fashion by creating a new node-pool and specifying that the KPO pods are to be run in the new node-pool


### How do I reuse code between DAG files?
Put your utility functions in a local Python library and import the functions. You can reference the functions in any DAG in the dags/ folder.

### How do I minimize the risk of different definitions arising?
For example, I have two teams that want to aggregate raw data into revenue metrics. The teams write two slightly different tasks that accomplish the same thing.

Define libraries to work with the revenue data so that the DAG implementers must clarify the definition of revenue that’s being aggregated.

### How do I set dependencies between DAGs?
This depends on how you want to define the dependency.

If you have two DAGs (DAG A and DAG B) and you want DAG B to trigger after DAG A, you can put a TriggerDagRunOperator at the end of Dag A.
If DAG B depends only on an artifact that DAG A generates, such as a Pub/Sub message, then a sensor might work better.
If DAG B is integrated closely with DAG A, you might be able to merge the two DAGs into one DAG.

### How do I pass unique run IDs to a DAG and its tasks?
For example, I want to pass Dataproc cluster names and file paths.

You can generate a random unique ID by returning str(uuid.uuid4()) in a PythonOperator. This will place the ID into xcoms so that you can refer to the ID in other operators via templated fields.

Before generating a uuid, consider whether a DagRun-specific ID would be more valuable. You can also reference these IDs in Jinja substitutions via macros.


### Where do I draw the line between tasks in a DAG?
Each task should be an idempotent unit of work. Consequently, you should avoid encapsulating a multi-step workflow within a single task, such as a complex program running in a PythonOperator.

The Airflow-native mechanism for re-using workflow definition code is the SubDagOperator. However, there are caveats. For information, see Should I use the SubDagOperator.

### Should I define multiple tasks in a single DAG to aggregate data from multiple sources?
For example, I have multiple tables with raw data and want to create daily aggregates for each table. The tasks are not dependent on each other. Should I create one task and DAG for each table or create one general DAG?

If you are okay with each task sharing the same DAG-level properties, such as schedule_interval, then it makes sense to define multiple tasks in a single DAG. Otherwise, to minimize code repetition, multiple DAGs can be generated from a single Python module by placing them into the module’s globals.

### How do I limit the number of concurrent tasks running in a DAG?
For example, I want to avoid exceeding API usage limits/quotas or avoid running too many simultaneous processes.

You can define Airflow pools in the Airflow web UI and associate tasks with existing pools in your DAGs.


##  How is SQL Azure different than SQL server?

SQL Azure is a cloud-based service and so it has own set of pros and cons when compared to SQL server. SQL Azure service benefits include on-demand provisioning, high availability, reduced management overhead and scalability. But SQL Azure abstracts some details from the subscriber which can be good or bad which depends on the context of the need.


## How many replicas are maintained for each SQL Azure database?

For each database, three replicas are maintained for each database that one provisions. One of them is a primary replica. All read/write happen on primary replica and other replicas are kept in sync with the primary replica. If for some reason, primary goes down, another replica is promoted to primary. All this happens under the hood.

##  How can we migrate from SQL server to SQL Azure?

For Data Migration, we can use BCP or SSIS. And for schema Migration, we can use Generate Script Wizard. Also, we could use a Tool called SQL Azure migration wizard.

## Which tools are available to manage SQL Azure databases and servers?

We can manage SQL Azure database using SQL server management server 2008 R2. Also, we can manage SQL Azure databases and servers through a Silverlight app integrated in Azure management portal.

##  Tell me something about security and SQL Azure.

SQL Azure service allows blocking a request based on its IP address through SQL Azure firewall. It uses SQL server Authentication mechanism to authenticate connections. Also connections to SQL Azure are SSL-encrypted by default.

##  How do we synchronize On-Premise SQL server with SQL Azure?

We could use a No code solution called DATA SYNC (currently in community technology preview) to synchronize on-premise SQL server with SQL Azure. We can also develop custom solutions using SYNC framework.

## How do we Backup SQL Azure Data?

SQL Azure keeps three replicas of a database to tackle hardware level issues. To tackle user level errors, we can use COPY command that allows us to create a replica of a SQL Azure database. We can also backup SQL Azure data to local SQL server using BCP, SSIS, etc. but as of now, point in time recovery is not supported.


## What is the current limitation of the size of SQL Azure DB?

The maximum size of a SQL Azure database is 50 GB.

## How do you handle datasets larger than 50 GB?

As of now, we have to build the custom solution at the application level that can handle scale out of underlying SQL Azure databases. But Microsoft has announced, SQL Azure Federations that will assist scaling out of SQL Azure databases. And scale out means that we are splitting the data into smaller subsets spread across multiple databases.

## What happens when the SQL Azure database reaches Max Size?

Read operations continue to work but create/insert/update operations are throttled. You can drop/delete/truncate data.

## How many databases can we create on a single server?

150 databases (including master database) can be created in a single SQL Azure server.

## What is Power BI?

Power BI is a cloud-based data sharing environment. Once you have developed reports using Power Query, Power Pivot and Power View, you can share your insights with your colleagues. This is where Power BI enters the equation. Power BI, which technically is an aspect of SharePoint online, lets you load Excel workbooks into the cloud and share them with a chosen group of co-workers. Not only that, but your colleagues can interact with your reports to apply filters and slicers to highlight data. They are completed by Power BI, a simple way of sharing your analysis and insights from the Microsoft cloud.

Power BI features allow you to:

Share presentations and queries with your colleagues.
Update your Excel file from data sources that can be on-site or in the cloud.
Display the output on multiple devices. This includes PCs, tablets, and HTML 5-enabled mobile devices that use the Power BI app.
Query your data using natural language processing (or Q&A, as it is known).

## What data sources can Power BI connect to?
Ans: The list of data sources for Power BI is extensive, but it can be grouped into the following:

Files: Data can be imported from Excel (.xlsx, xlxm), Power BI Desktop files (.pbix) and Comma Separated Value (.csv).
Content Packs: It is a collection of related documents or files that are stored as a group. In Power BI, there are two types of content packs, firstly those from services providers like Google Analytics, Marketo or Salesforce and secondly those created and shared by other users in your organization.
Connectors to databases and other datasets such as Azure SQL, Databaseand SQL, Server Analysis Services tabular data, etc.

## What are Building Blocks in Power BI?
Ans: The following are the Building Blocks (or) key components of Power BI:

Visualizations: Visualization is a visual representation of data.
Example: Pie Chart, Line Graph, Side by Side Bar Charts, Graphical Presentation of the source data on top of Geographical Map, Tree Map, etc.
Datasets: Dataset is a collection of data that Power BI uses to create its visualizations.
Example: Excel sheets, Oracle or SQL server tables.
Reports: Report is a collection of visualizations that appear together on one or more pages.
Example: Sales by Country, State, City Report, Logistic Performance report, Profit by Products report etc.
Dashboards: Dashboard is single layer presentation of multiple visualizations, i.e we can integrate one or more visualizations into one page layer.
Example: Sales dashboard can have pie charts, geographical maps and bar charts.
Tiles: Tile is a single visualization in a report or on a dashboard.
Example: Pie Chart in Dashboard or Report.

## What are the different types of filters in Power BI Reports?

Ans: Power BI provides variety of option to filter report, data and visualization. The following are the list of Filter types.

Visual-level Filters: These filters work on only an individual visualization, reducing the amount of data that the visualization can see. Moreover, visual-level filters can filter both data and calculations.
Page-level Filters: These filters work at the report-page level. Different pages in the same report can have different page-level filters.
Report-level Filters: There filters work on the entire report, filtering all pages and visualizations included in the report.
We know that Power BI visual have interactions feature, which makes filtering a report a breeze. Visual interactions are useful, but they come with some limitations:

The filter is not saved as part of the report. Whenever you open a report, you can begin to play with visual filters but there is no way to store the filter in the saved report.
The filter is always visible. Sometimes you want a filter for the entire report, but you do not want any visual indication of the filter being applied.

## What is DAX?
Ans: To do basic calculation and data analysis on data in power pivot, we use Data Analysis Expression (DAX). It is formula language used to compute calculated column and calculated field.

DAX works on column values.
DAX can not modify or insert data.
We can create calculated column and measures with DAX  but we can not calculate rows using DAX.
Sample DAX formula syntax:

For the measure named Total Sales, calculate (=) the SUM of values in the [SalesAmount] column in the Sales table.

## What are the most common DAX Functions used?
Ans: Below are some of the most commonly used DAX function: 

SUM, MIN, MAX, AVG, COUNTROWS, DISTINCTCOUNT
IF, AND, OR, SWITCH
ISBLANK, ISFILTERED, ISCROSSFILTERED
VALUES, ALL, FILTER, CALCULATE,
UNION, INTERSECT, EXCEPT, NATURALINNERJOIN, NATURALLEFTEROUTERJOIN,
SUMMARIZECOLUMNS, ISEMPTY,
VAR (Variables)
GEOMEAN, MEDIAN, DATEDIFF

## What is Power Query?
Ans: Power query is a ETL Tool used to shape, clean and transform data using intuitive interfaces without having to use coding. It helps the user to:

Import Data from wide range of sources from files, databases, big data, social media data, etc.
Join and append data from multiple data sources. 
Shape data as per requirement by removing and adding data.

## What are the data destinations for Power Queries?
Ans: There are two destinations for output we get from power query:

Load to a table in a worksheet.
Load to the Excel Data Model.

## Can SQL and Power Query/Query Editor be used together?
Ans: Yes, a SQL statement can be defined as the source of a Power Query/M function for additional processing/logic. This would be a good practice to ensure that an efficient database query is passed to the source and avoid unnecessary processing and complexity
by the client machine and M function.

## What are the primary requirement for a table to be used in Power Map?
Ans: For a data to be consumed in power map there should be location data like:

Latitude/Longitude pair
Street, City, Country/Region, Zip Code/Postal Code, and State/Province, which can be geolocated by Bing
The primary requirement for the table is that it contains unique rows. It must also contain location data, which can be in the form of a Latitude/Longitude pair, although this is not a requirement. You can use address fields instead, such as Street, City, Country/Region, Zip Code/Postal Code, and State/Province, which can be geolocated by Bing.

## Compare QlikView with Tableau

Criteria|Tableau|QlikView 
----|----|----
Data integration |Exceptional|	Good
Working with multidimensional data	|Very Good	|Good
Support for PowerPoint|	Available	|Not available
Visual Drilldown	|Good	|Very Good
Scalability	|Good	|Limited by RAM

## What are Filters? How many types of Filters are there in Tableau?
A Filter restricts unnecessary data; it shows the exact data we want. Basically, Filters are of three types:

Quick Filter
Context Filter
Datasource Filter

## How is the Context Filter different from other Filters?
Whenever we create a Context Filter, Tableau will create a temporary table for this particular Filter set and other Filters will be applied on the Context Filter data like cascade parameters.
Suppose, we have created a Context Filter on countries, USA and India, Tableau will create a temporary table for these two countries’ data and if we have any other Filters other will be applied on these two countries’ data if we don’t have any Context Filter, each record will check for all Filters.

## What is the disadvantage of Context Filters?
The Context Filter is not frequently changed by the user—if the Filter is changed, the database must be recomputed and the temporary table has to be rewritten, slowing performance.
When we set a dimension to context, Tableau creates a temporary table that will require a reload each time the view is initiated. For Excel, Access, and text data sources, the temporary table created is in an Access table format. For SQL Server, MySQL, and Oracle data sources, we must have permission to create a temporary table on our server. For a multidimensional data source, or cubes, temporary tables are not created, and Context Filters defined which Filters are independent and which are dependent.

## What are the five main products offered by Tableau?
Tableau offers five main products:

Tableau Desktop
Tableau Server
Tableau Online
Tableau Reader
Tableau Public

## What is data visualization?
Data visualization refers to the techniques used to communicate data or information by encoding it as visual objects (e.g., points, lines, or bars) contained in graphics.

## Why Tableau?
Whether our data is in an on-premise database, a database, a data warehouse, a cloud application, or in an Excel file, we can analyze it with Tableau. We can create views of our data and share it with colleagues, customers, and partners. We can use Tableau to blend it with other data, and we can keep our data up to date automatically.


## What is aggregation and disaggregation of data?
Suppose, we have data like below:

Eid Ename Salary Dept
1.abc 2000 java
2.bbc 3000 .net
3.Krishna 2500 java
Madhu 300
5.Vamshi 3000 mainframes
1.abc 1000 testing
2.bbc 3000 tableau
3.krishna 5000.net
4.Madhu 7000 testing
vanshi 9000 tableau
1 abc 11000 Mainframes
2 bbc 13000testing
3 krishna 15000 java
4 Madhu 17000 .nte
5 vamshi 19000.net

Aggregation: To display aggregate data
Sum/avg salary by each individual employee
Drag ename on column and salary on rows, and we will get the sum (salary) of each and individual employee
Now, change the measure type as Avg

Choose salary option: choose measure types as ‘Avg’

Disaggregation: To display each and every transaction

When we look at the aggregated data in the views above, each bar represents all transactions for a specific employee summed up or averaged into a single value. Now, say, we want to see the individual salary transactions for each employee. We can create a view like that by selecting Analysis > Aggregate Measures.

## How to combine two Excel files with the same fields but different data (different years)?
Suppose, we have five different Excel files (2007.xls, 2008.xls, … 2011.xls) with the same fields (film name, genre, budget, rating, profitability, etc.) but with data of different years (2007 to 2011). Can someone tell me how can I combine the film name, genre, and profitability so that I can see the visualization of 2007 to 2011 in a single chart?

## What is the difference between joining and blending in Tableau?
Joins in Tableau

Suppose, our client is in the healthcare domain and using SQL Server as their database. In SQL Server, there may be many Tableau-like Claims Tables, Rejected Claims Table, Customer Table, etc. Now, the client wants to know the customer-wise claims and the customer-wise rejected claims table using the Joins. Join is a query that combines the data from two or more tables by making use of the Join condition.

We can join a maximum of 32 tables; it is not possible to combine more than 32 tables.

In Tableau, Joins can be performed in two ways:

By making use of common columns
By making use of common data types
If we create Joins on the fields, in Tableau, all the table names are suffixed with $. While performing Joins on multiple tables, always go with the less amount of data tables, so that we can improve the performance.

In Tableau, Joins are divided into two types:

Equi Join
Non-equi Join
Equi Join

In the Join condition, if we are using equality (‘=’) operator, then such a kind of join is called Equi Join. Equi Join is further divided into three types:

Inner Join: Inner Join will load the only matching records from both tables. Below is the Inner Join condition:
Tableaa.id = Tableb.id
Outer Join: Outer Join is further divided into three types:
Left Outer Join: Displays the complete data from the left table + matching records from the right
Condition:
tablea.id(+)
Right Outer Join: Displays the complete data from the right table + matching records from the left
Condition:
tablea.id(+)=tableb.id
Full Outer Join: Loads the complete data from the left table and the right table
Condition:
Table A full outer join Table B ON tablea.id= tableb.id
Self-join: If we are performing Join to a table with itself such a kind of Join is called a Self-join.
Non-equi Join

In the Join condition, if we are using operators apart from the equality (‘=’) operator (such as, <, >, <=, >=, and =!), then such a kind of Join is called Non-equi Join.

Data Blending in Tableau

Consider the same client. Suppose, they are operating their services in Asia, Europe, NA, and so on, and they are maintaining Asia data in SQL, Europe data in SQL Server, and NA data in MySQL.

Now, our client wants to analyze their business across the world in a single worksheet. In this case, we can’t perform a Join. Here, we have to make use of the data blending concept.

Normally, in Tableau, we can perform the analysis on a single data server. If we want to perform the analysis of data from multiple data sources in a single sheet, then we have to make use of this new concept called data blending.

Data blending mixes the data from different data sources and allows users to perform the analysis in a single sheet. ‘Blending’ means ‘mixing’ and when we are mixing the data sources, then it is called data blending.

Rules to Perform Data Blending

In order to perform data blending, there are a few rules:

If we are performing data blending on two data sources, these two data sources should have at least one common dimension.
In that common dimension, at least one value should be matching.
In Tableau, we can perform data blending in two ways.

Automatic way: Here, Tableau automatically defines the relationship between the two data sources based on the common dimensions and based on the matching values, and the relationship is indicated in orange.
Custom or Manual way: In the manual or custom way, the user needs to define the relationship manually.
Data Blending Functionality

All the primary and secondary data sources are linked by a specific relationship.
While performing data blending, each worksheet has a primary connection, and optionally it might contain several secondary connections.
All the primary connections are indicated in blue in the worksheet and all the secondary connections with an orange-colored tick mark.
In data blending, one sheet contains one primary data source and it can contain n number of secondary data sources.

## What are Dimensions and Facts?
Dimensions are nothing but the descriptive text columns. Example: product name, city, etc.
Facts are the measures (numerical values). Example: sales, profit, etc.

## What is the difference between heat map and treemap?
A heat map is a great way to compare categories using color and size. In this, we can compare two different measures.
A treemap is a very powerful visualization, particularly used for illustrating hierarchical (tree-structured) data and for visualizing a part of or a whole relationship.

## What is the different between twb and twbx file extensions. Please explain.
The file extension .twb is a live connection; it points to the data source. The user receiving .twb needs permission to access the said data source and no data is included.

On the other hand, .twbx takes the data offline and stores it as a package or zip-like file, thereby eradicating the need for permissions.

## What is the use of the new custom SQL query in Tableau?
Custom SQL query is written after connecting to data for pulling the data in a structured view. For example, suppose, we have 50 columns in a table, but we need just 10 columns only. So instead of taking 50 columns, we can write a SQL query. The performance will increase.

## What are the similarities and differences between Tableau and Palantir?
Palantir and Tableau are very different. Palantir has its roots in large data computer science problems involving security, payments, fraud detection, and the like. Its customers/investors include PayPal, CIA, and others.

Tableau is a visualization player, with roots in Stanford University Research. Its Visual Query Language (VizQL) allows users to build visualizations on top of the standard data warehouses or spreadsheets.

## How can we combine a database and the flat file data in Tableau Desktop?
Connect data twice, once for database tables and then for the flat file. The Data->Edit Relationships
Give a Join condition on the common column from DB tables to the flat file


## What is data modeling?
Data modeling is the analysis of data objects that are used in a business or other context and the identification of the relationships among these data objects. Data modeling is the first step in performing object-oriented programming.



## Load CSV data into BigQuery via CLI

```
  bq load \
    --source_format=CSV \
    --skip_leading_rows=2
    mydataset.mytable \
    gs://mybucket/mydata.csv \
    ./myschema.json
```


## Load CSV data into BigQuery via Go

```
import (
        "context"
        "fmt"

        "cloud.google.com/go/bigquery"
)

// importCSVExplicitSchema demonstrates loading CSV data from Cloud Storage into a BigQuery
// table and providing an explicit schema for the data.
func importCSVExplicitSchema(projectID, datasetID, tableID string) error {
        // projectID := "my-project-id"
        // datasetID := "mydataset"
        // tableID := "mytable"
        ctx := context.Background()
        client, err := bigquery.NewClient(ctx, projectID)
        if err != nil {
                return fmt.Errorf("bigquery.NewClient: %v", err)
        }
        defer client.Close()

        gcsRef := bigquery.NewGCSReference("gs://cloud-samples-data/bigquery/us-states/us-states.csv")
        gcsRef.SkipLeadingRows = 1
        gcsRef.Schema = bigquery.Schema{
                {Name: "name", Type: bigquery.StringFieldType},
                {Name: "post_abbr", Type: bigquery.StringFieldType},
        }
        loader := client.Dataset(datasetID).Table(tableID).LoaderFrom(gcsRef)
        loader.WriteDisposition = bigquery.WriteEmpty

        job, err := loader.Run(ctx)
        if err != nil {
                return err
        }
        status, err := job.Wait(ctx)
        if err != nil {
                return err
        }

        if status.Err() != nil {
                return fmt.Errorf("job completed with error: %v", status.Err())
        }
        return nil
}
```

## Load CSV data into BigQuery in python

```
# from google.cloud import bigquery
# client = bigquery.Client()
# dataset_id = 'my_dataset'

dataset_ref = client.dataset(dataset_id)
job_config = bigquery.LoadJobConfig()
job_config.schema = [
    bigquery.SchemaField("name", "STRING"),
    bigquery.SchemaField("post_abbr", "STRING"),
]
job_config.skip_leading_rows = 1
# The source format defaults to CSV, so the line below is optional.
job_config.source_format = bigquery.SourceFormat.CSV
uri = "gs://cloud-samples-data/bigquery/us-states/us-states.csv"

load_job = client.load_table_from_uri(
    uri, dataset_ref.table("us_states"), job_config=job_config
)  # API request
print("Starting job {}".format(load_job.job_id))

load_job.result()  # Waits for table load to complete.
print("Job finished.")

destination_table = client.get_table(dataset_ref.table("us_states"))
print("Loaded {} rows.".format(destination_table.num_rows))
```

## How to stream insert data into BigQuery

```
import (
        "context"
        "fmt"

        "cloud.google.com/go/bigquery"
)

// Item represents a row item.
type Item struct {
        Name string
        Age  int
}

// Save implements the ValueSaver interface.
func (i *Item) Save() (map[string]bigquery.Value, string, error) {
        return map[string]bigquery.Value{
                "full_name": i.Name,
                "age":       i.Age,
        }, "", nil
}

// insertRows demonstrates inserting data into a table using the streaming insert mechanism.
func insertRows(projectID, datasetID, tableID string) error {
        // projectID := "my-project-id"
        // datasetID := "mydataset"
        // tableID := "mytable"
        ctx := context.Background()
        client, err := bigquery.NewClient(ctx, projectID)
        if err != nil {
                return fmt.Errorf("bigquery.NewClient: %v", err)
        }
        defer client.Close()

        inserter := client.Dataset(datasetID).Table(tableID).Inserter()
        items := []*Item{
                // Item implements the ValueSaver interface.
                {Name: "Phred Phlyntstone", Age: 32},
                {Name: "Wylma Phlyntstone", Age: 29},
        }
        if err := inserter.Put(ctx, items); err != nil {
                return err
        }
        return nil
}
```


## How do query via CLI

```
bq query \
--destination_table mydataset.mytable \
--use_legacy_sql=false \
'SELECT
  name,
  number
FROM
  `bigquery-public-data.usa_names.usa_1910_current`
WHERE
  gender = "M"
ORDER BY
  number DESC'

```


## How to query via Go:

```
import (
        "context"
        "fmt"
        "io"

        "cloud.google.com/go/bigquery"
        "google.golang.org/api/iterator"
)

// queryBasic demonstrates issuing a query and reading results.
func queryBasic(w io.Writer, projectID string) error {
        // projectID := "my-project-id"
        ctx := context.Background()
        client, err := bigquery.NewClient(ctx, projectID)
        if err != nil {
                return fmt.Errorf("bigquery.NewClient: %v", err)
        }
        defer client.Close()

        q := client.Query(
                "SELECT name FROM `bigquery-public-data.usa_names.usa_1910_2013` " +
                        "WHERE state = \"TX\" " +
                        "LIMIT 100")
        // Location must match that of the dataset(s) referenced in the query.
        q.Location = "US"
        // Run the query and print results when the query job is completed.
        job, err := q.Run(ctx)
        if err != nil {
                return err
        }
        status, err := job.Wait(ctx)
        if err != nil {
                return err
        }
        if err := status.Err(); err != nil {
                return err
        }
        it, err := job.Read(ctx)
        for {
                var row []bigquery.Value
                err := it.Next(&row)
                if err == iterator.Done {
                        break
                }
                if err != nil {
                        return err
                }
                fmt.Fprintln(w, row)
        }
        return nil
}
```

## How to query via python

```


from google.cloud import bigquery

# Construct a BigQuery client object.
client = bigquery.Client()

query = """
    SELECT name, SUM(number) as total_people
    FROM `bigquery-public-data.usa_names.usa_1910_2013`
    WHERE state = 'TX'
    GROUP BY name, state
    ORDER BY total_people DESC
    LIMIT 20
"""
query_job = client.query(query)  # Make an API request.

print("The query data:")
for row in query_job:
    # Row values can be accessed by field name or index.
    print("name={}, count={}".format(row[0], row["total_people"]))

```

## Query BigTable data from BigQuery

```
bq query \
--use_legacy_sql=false \
--external_table_definition=follows::/tmp/follows_def \
'SELECT
  COUNT(rowkey)
 FROM
   follows'
```


## Query Cloud Storage from BigQuery

```
# from google.cloud import bigquery
# client = bigquery.Client()
# dataset_id = 'my_dataset'

# Configure the external data source
dataset_ref = client.dataset(dataset_id)
table_id = "us_states"
schema = [
    bigquery.SchemaField("name", "STRING"),
    bigquery.SchemaField("post_abbr", "STRING"),
]
table = bigquery.Table(dataset_ref.table(table_id), schema=schema)
external_config = bigquery.ExternalConfig("CSV")
external_config.source_uris = [
    "gs://cloud-samples-data/bigquery/us-states/us-states.csv"
]
external_config.options.skip_leading_rows = 1  # optionally skip header row
table.external_data_configuration = external_config

# Create a permanent table linked to the GCS file
table = client.create_table(table)  # API request

# Example query to find states starting with 'W'
sql = 'SELECT * FROM `{}.{}` WHERE name LIKE "W%"'.format(dataset_id, table_id)

query_job = client.query(sql)  # API request

w_states = list(query_job)  # Waits for query to finish
print("There are {} states with names starting with W.".format(len(w_states)))
```


## Query Google Drive data from BigQuery

```
from google.cloud import bigquery
import google.auth

# Create credentials with Drive & BigQuery API scopes.
# Both APIs must be enabled for your project before running this code.
credentials, project = google.auth.default(
    scopes=[
        "https://www.googleapis.com/auth/drive",
        "https://www.googleapis.com/auth/bigquery",
    ]
)

# TODO(developer): Construct a BigQuery client object.
client = bigquery.Client(credentials=credentials, project=project)
```


## Dataflow & Apache Beam questions

### What is Apache Beam?

Apache Beam is an evolution of the Dataflow model created by Google to process massive amounts of data. The name Beam (Batch + strEAM) comes from the idea of having a unified model for both batch and stream data processing. Programs written using Beam can be executed in different processing frameworks (via runners) using a set of different IOs.

Beam is an API that separates the building of a data processing pipeline from the actual engine on which it would run. It includes abstractions for specifying the data pipeline, the actual data stream (akin to Spark's RDDs), transformation functions, "runners" (the compute engine), and the sources and targets. It's one of a growing number of approaches for flattening the Lambda architecture, so you can combine real time and batch processing (and interactive as well) on the same code base and cluster.

Beam extracts the SDK and dataflow model from Google's own Cloud Dataflow service. On closer inspection, support for the Beam programming model is roughly 70 percent complete across Apache Apex, Flink, and Spark Streaming engines. The biggest gap is with functions dependent on true stream processing (the ability to process one event at time and set discrete time windows), where Spark Streaming's microbatch capabilities either fall short or require workarounds.

### Why we actually need Apache beam when we already have Hadoop/Spark/Flink?
There are many frameworks like Hadoop, Spark, Flink, Google Cloud Dataflow, etc that came into existence. But there has been no unified API that binds all these frameworks and data sources, and provide an abstraction to the application logic from big data ecosystem. Apache Beam framework provides an abstraction between your application logic and the big data ecosystem.

### What is Apache Flink?

Apache Flink is a framework and distributed processing engine for stateful computations over unbounded and bounded data streams. Flink has been designed to run in all common cluster environments, perform computations at in-memory speed and at any scale.

Here, we explain important aspects of Flink’s architecture.

Process Unbounded and Bounded Data
Any kind of data is produced as a stream of events. Credit card transactions, sensor measurements, machine logs, or user interactions on a website or mobile application, all of these data are generated as a stream.

Data can be processed as unbounded or bounded streams.

Unbounded streams have a start but no defined end. They do not terminate and provide data as it is generated. Unbounded streams must be continuously processed, i.e., events must be promptly handled after they have been ingested. It is not possible to wait for all input data to arrive because the input is unbounded and will not be complete at any point in time. Processing unbounded data often requires that events are ingested in a specific order, such as the order in which events occurred, to be able to reason about result completeness.

Bounded streams have a defined start and end. Bounded streams can be processed by ingesting all data before performing any computations. Ordered ingestion is not required to process bounded streams because a bounded data set can always be sorted. Processing of bounded streams is also known as batch processing.

### What is Apache Apex

Apex is a Hadoop YARN native big data processing platform, enabling real time stream as well as batch processing for your big data. Apex provides the following benefits:

* High scalability and performance
* Fault tolerance and state management
* Hadoop-native YARN & HDFS implementation
* Event processing guarantees
* Separation of functional and operational concerns
* Simple API supports generic Java code

Platform has been demonstated to scale linearly across Hadoop clusters under extreme loads of billions of events per second. Hardware and process failures are quickly recovered with HDFS-backed checkpointing and automatic operator recovery, preserving application state and resuming execution in seconds. Functional and operational specifications are separated. Apex provides a simple API, which enables users to write generic, reusable code. The code is dropped in as-is and platform automatically handles the various operational concerns, such as state management, fault tolerance, scalability, security, metrics, etc. This frees users to focus on functional development, and lets platform provide operability support.

The core Apex platform is supplemented by Malhar, a library of connector and logic functions, enabling rapid application development. These operators and modules provide access to HDFS, S3, NFS, FTP, and other file systems; Kafka, ActiveMQ, RabbitMQ, JMS, and other message systems; MySql, Cassandra, MongoDB, Redis, HBase, CouchDB, generic JDBC, and other database connectors. In addition to the operators, the library contains a number of demos applications, demonstrating operator features and capabilities.

Here is a comparison between Spark and Flink https://www.developintelligence.com/blog/2017/02/comparing-contrasting-apache-flink-vs-spark/

### What are five main concepts in beam?

* Pipeline: A Pipeline encapsulates the workflow of your entire data processing tasks from start to finish. This includes reading input data, transforming that data, and writing output data. All Beam driver programs must create a Pipeline. When you create the Pipeline, you must also specify the execution options that tell the Pipeline where and how to run.
* PCollection: A PCollection represents a distributed data set that your Beam pipeline operates on. The data set can be bounded, meaning it comes from a fixed source like a file, or unbounded, meaning it comes from a continuously updating source via a subscription or other mechanism
* PTransform: A PTransform represents a data processing operation, or a step, in your pipeline. Every PTransform takes one or more PCollection objects as input, performs a processing function that you provide on the elements of that PCollection, and produces zero or more output PCollection objects.
* ParDo: ParDo is a Beam transform for generic parallel processing. The ParDo processing paradigm is similar to the “Map” phase of a Map/Shuffle/Reduce-style algorithm: a ParDo transform considers each element in the input PCollection, performs some processing function (your user code) on that element, and emits zero, one, or multiple elements to an output PCollection.
* DoFn: A DoFn applies your logic in each element in the input PCollection and lets you populate the elements of an output PCollection. To be included in your pipeline, it’s wrapped in a ParDo PTransform.

### Is it possible to share data across pipeline instances in Google Cloud dataflow?

There is no Dataflow-specific cross pipeline communication mechanism for sharing data or processing context between pipelines. You can use durable storage like Cloud Storage or an in-memory cache like App Engine to share data between pipeline instances.


### In Cloud dataflow, is it possible to access my job's worker machines (Compute Engine VMs) while my pipeline is running?
You can view the VM instances for a given pipeline by using the Google Cloud Console. From there, you can use SSH to access each instance. However, once your job either completes or fails, the Dataflow service will automatically shut down and clean up the VM instances.

### In the Cloud Dataflow Monitoring Interface, why don't I see Reserved CPU Time for my streaming job?
The Dataflow service reports Reserved CPU Time after jobs are completed. For unbounded jobs, this means Reserved CPU time is only reported after jobs have been cancelled or have failed.

### In the Cloud Dataflow Monitoring Interface, why are the job state and watermark information unavailable for recently updated streaming jobs?
The Update operation makes several changes that take a few minutes to propagate to the Dataflow Monitoring Interface. Try refreshing the monitoring interface 5 minutes after updating your job.


### Can I pass additional (out-of-band) data into an existing ParDo operation?
Yes. There are several patterns to follow, depending on your use case:

* You can serialize information as fields in your DoFn subclass.
* Any variables referenced by the methods in an anonymous DoFn will be automatically serialized.
* You can compute data inside DoFn.startBundle().
* You can pass in data via ParDo.withSideInputs.


## Data warehouses

### What are differences between Operational database and Data warehouse?


The Operational Database is the source of information for the data warehouse. It includes detailed information used to run the day to day operations of the business. The data frequently changes as updates are made and reflect the current value of the last transactions.

Operational Database Management Systems also called as OLTP (Online Transactions Processing Databases), are used to manage dynamic data in real-time.

Data Warehouse Systems serve users or knowledge workers in the purpose of data analysis and decision-making. Such systems can organize and present information in specific formats to accommodate the diverse needs of various users. These systems are called as Online-Analytical Processing (OLAP) Systems.

Data Warehouse and the OLTP database are both relational databases. However, the goals of both these databases are different.


### What is ETL vs ELT?

Extract, Transform and Load is the technique of extracting the record from sources (which is present outside or on-premises, etc.) to a staging area, then transforming or reformatting with business manipulation performed on it in order to fit the operational needs or data analysis, and later loading into the goal or destination databases or data warehouse.

ELT stands for Extract, Load and Transform is the various sight while looking at data migration or movement. ELT involves the extraction of aggregate information from the source system and loading to the target method instead of transformation between the extraction and loading phase. Once the data is copied or loaded into the target method, then change takes place.

https://www.javatpoint.com/data-warehouse-etl-vs-elt

### what are differences between OLTP and OLAP?

OLTP System handle with operational data. Operational data are those data contained in the operation of a particular system. Example, ATM transactions and Bank transactions, etc.

OLAP handle with Historical Data or Archival Data. Historical data are those data that are achieved over a long period. For example, if we collect the last 10 years information about flight reservation, the data can give us much meaningful data such as the trends in the reservation. This may provide useful information like peak time of travel, what kind of people are traveling in various classes (Economy/Business) etc.

The major difference between an OLTP and OLAP system is the amount of data analyzed in a single transaction. Whereas an OLTP manage many concurrent customers and queries touching only an individual record or limited groups of files at a time. An OLAP system must have the capability to operate on millions of files to answer a single query.



### What is Data Cube?
When data is grouped or combined in multidimensional matrices called Data Cubes. The data cube method has a few alternative names or a few variants, such as "Multidimensional databases," "materialized views," and "OLAP (On-Line Analytical Processing)."

The general idea of this approach is to materialize certain expensive computations that are frequently inquired.

### What are some OLAP operations?

* The roll-up operation (also known as drill-up or aggregation operation) performs aggregation on a data cube, by climbing down concept hierarchies, i.e., dimension reduction. Roll-up is like zooming-out on the data cubes. 
* The drill-down operation (also called roll-down) is the reverse operation of roll-up. Drill-down is like zooming-in on the data cube. It navigates from less detailed record to more detailed data. Drill-down can be performed by either stepping down a concept hierarchy for a dimension or adding additional dimensions.
* A slice is a subset of the cubes corresponding to a single value for one or more members of the dimension. For example, a slice operation is executed when the customer wants a selection on one dimension of a three-dimensional cube resulting in a two-dimensional site. So, the Slice operations perform a selection on one dimension of the given cube, thus resulting in a subcube.
* The dice operation describes a subcube by operating a selection on two or more dimension.
* The pivot operation is also called a rotation. Pivot is a visualization operations which rotates the data axes in view to provide an alternative presentation of the data. It may contain swapping the rows and columns or moving one of the row-dimensions into the column dimensions.

Other OLAP operations may contain ranking the top-N or bottom-N elements in lists, as well as calculate moving average, growth rates, and interests, internal rates of returns, depreciation, currency conversions, and statistical tasks.

OLAP offers analytical modeling capabilities, containing a calculation engine for determining ratios, variance, etc. and for computing measures across various dimensions. It can generate summarization, aggregation, and hierarchies at each granularity level and at every dimensions intersection. OLAP also provide functional models for forecasting, trend analysis, and statistical analysis. In this context, the OLAP engine is a powerful data analysis tool.

### what are star and snowflake schemas?
Star Schema
* In a star schema, the fact table will be at the center and is connected to the dimension tables.
* The tables are completely in a denormalized structure.
* SQL queries performance is good as there is less number of joins involved.
* Data redundancy is high and occupies more disk space.

Snowflake Schema
* A snowflake schema is an extension of star schema where the dimension tables are connected to one or more dimensions.
* The tables are partially denormalized in structure.
* The performance of SQL queries is a bit less when compared to star schema as more number of joins are involved.
* Data redundancy is low and occupies less disk space when compared to star schema.

https://www.javatpoint.com/data-warehouse-star-schema-vs-snowflake-schema




### What is dimensional modeling?

Dimensional modeling represents data with a cube operation, making more suitable logical data representation with OLAP data management. The perception of Dimensional Modeling was developed by Ralph Kimball and is consist of "fact" and "dimension" tables.

In dimensional modeling, the transaction record is divided into either "facts," which are frequently numerical transaction data, or "dimensions," which are the reference information that gives context to the facts. For example, a sale transaction can be damage into facts such as the number of products ordered and the price paid for the products, and into dimensions such as order date, user name, product number, order ship-to, and bill-to locations, and salesman responsible for receiving the order.

### What are slowly changing dimensions in Data warehouse applications?

What are the types of SCD?

Very simply, there are 6 types of Slowly Changing Dimension that are commonly used, they are as follows:

* Type 0 – Fixed Dimension
No changes allowed, dimension never changes
* Type 1 – No History
Update record directly, there is no record of historical values, only current state
* Type 2 – Row Versioning
Track changes as version records with current flag & active dates and other metadata
* Type 3 – Previous Value column
Track change to a specific attribute, add a column to show the previous value, which is updated as further changes occur
* Type 4 – History Table
Show current value in dimension table but track all changes in separate table
* Type 6 – Hybrid SCD

Utilise techniques from SCD Types 1, 2 and 3 to track change
In reality, only types 0, 1 and 2 are widely used, with the others reserved for very specific requirements. Confusingly, there is no SCD type 5 in commonly agreed definitions.

After you have implemented your chosen dimension type, you can then point your fact records at the relevant business or surrogate key. Surrogate keys in these examples relate to a specific historical version of the record, removing join complexity from later data structures.

### What are Materialized Views in BigQuery?

BigQuery Materialized View are precomputed views that periodically cache results of a query for increased performance and efficiency. BigQuery leverages precomputed results from materialized views and whenever possible reads only delta changes from the base table to compute up-to-date results. Materialized views can be queried directly or can be used by the BigQuery optimizer to process queries to the base tables.

Queries that use materialized views are generally faster and consume less resources than queries that retrieve the same data only from the base table. Materialized views are helpful to significantly boost performance of workloads that have the characteristic of common and repeated queries.

### What are some example sources of data that can be loaded into BigQuery?

* From Cloud Storage
* From other Google services, such as Google Ad Manager and Google Ads
* From a readable data source (such as your local machine)
* By inserting individual records using streaming inserts
* Using DML statements to perform bulk inserts
* Using a BigQuery I/O transform in a Dataflow pipeline to write data to BigQuery

### What input data formats are supported in BigQuery?

BigQuery supports loading data from Cloud Storage and readable data sources in the following formats:

Cloud Storage:
* Avro
* CSV
* JSON (newline delimited only)
* ORC
* Parquet
* Datastore exports
* Firestore exports

Readable data source (such as your local machine):
* Avro
* CSV
* JSON (newline delimited only)
* ORC
* Parquet

The default source format for loading data is CSV. To load data that is stored in one of the other supported data formats, specify the format explicitly. When your data is loaded into BigQuery, it is converted into columnar format for Capacitor (BigQuery's storage format).


### What is external data source in BigQuery?

An external data source (also known as a federated data source) is a data source that you can query directly even though the data is not stored in BigQuery. Instead of loading or streaming the data, you create a table that references the external data source.

BigQuery offers support for querying data directly from:

* Bigtable
* Cloud Storage
* Google Drive
* Cloud SQL (beta)

## What is the command to initialize Gcloud SDK

```
gcloud init
```


## What is the cli command to list gcloud configuration

```
gcloud config list
```

## What is the cli command to view information about Cloud SDK installation and active SDK configuration?

```
gcloud info
```

## How to get a list of compute instances?

```
gcloud compute instances list
```

## What are zones vs regions?

## How to create a dataproc cluster?

```
gcloud dataproc clusters create example-cluster --regition=...
```

## How to submit a job to dataproc cluster?

```
gcloud dataproc jobs submit spark --cluster example-cluster --region=... --class org.apache.spark.example,SparkPi --jars file:///usr/lib/spark/examples/jars/spark-examples.jar -- 1000
```

## What are goroutines?  And how are they used?

## What are channels? How are they used?

## Explain Go Interfaces?

## How do you copy a slice?

Use copy() builtin.

```
a := []int{1, 2}
b := []int{3, 4}
check := a
copy(a, b)
fmt.Println(a, b, check)
// Output: [3 4] [3 4] [3 4]
```

## How do you copy a map?

You copy a map by traversing its keys. Yes, unfortunately, this is the simplest way to copy a map in Go:

```
a := map[string]bool{"A": true, "B": true}
b := make(map[string]bool)
for key, value := range a {
	b[key] = value
}
```


Following example copies just the description of the map:

```
a := map[string]bool{"A": true, "B": true}
b := map[string]bool{"C": true, "D": true}
check := a
a = b
fmt.Println(a, b, check)
// Output: map[C:true D:true] map[C:true D:true] map[A:true B:true]

```

## How do you copy an interface?

There’s no built-in way in Go to copy an interface. No, the reflect.DeepCopy() function does not exist.


## How do you compare two structs?


You can compare two structs with the == operator, as you would do with other simple types. Just make sure they do not contain any slices, maps, or functions, in which case the code will not be compiled.

```
type Foo struct {
	A int
	B string
	C interface{}
}
a := Foo{A: 1, B: "one", C: "two"}
b := Foo{A: 1, B: "one", C: "two"}

println(a == b)
// Output: true

type Bar struct {
	A []int
}
a := Bar{A: []int{1}}
b := Bar{A: []int{1}}

println(a == b)
// Output: invalid operation: a == b (struct containing []int cannot be compared)

```

## How do you compare two interfaces?

You can compare two interfaces with the == operator as long as the underlying types are “simple” and identical. Otherwise the code will panic at runtime:
```
var a interface{}
var b interface{}

a = 10
b = 10
println(a == b)
// Output: true

a = []int{1}
b = []int{2}
println(a == b)
// Output: panic: runtime error: comparing uncomparable type []int
Both structs and interfaces which contain maps, slices (but not functions) can be compared with the reflect.DeepEqual() function:

var a interface{}
var b interface{}

a = []int{1}
b = []int{1}
println(reflect.DeepEqual(a, b))
// Output: true

a = map[string]string{"A": "B"}
b = map[string]string{"A": "B"}
println(reflect.DeepEqual(a, b))
// Output: true

temp := func() {}
a = temp
b = temp
println(reflect.DeepEqual(a, b))
// Output: false
```

## How do you compare byte slices?

For comparing byte slices, there are nice helper functions in the bytes package: bytes.Equal(), bytes.Compare(), and bytes.EqualFold(). The latter is for comparing text strings disregarding the case, which are much faster than the reflect.DeepEqual().


## What is wrong with the following code snippet?

```
type Orange struct {
	Quantity int
}

func (o *Orange) Increase(n int) {
	o.Quantity += n
}

func (o *Orange) Decrease(n int) {
	o.Quantity -= n
}

func (o *Orange) String() string {
	return fmt.Sprintf("%v", o.Quantity)
}

func main() {
	var orange Orange
	orange.Increase(10)
	orange.Decrease(5)
	fmt.Println(orange)
}

```

This is a trick question because you might think this has something to do with the member variable Quantity being set incorrectly, but actually, it will be set to 5 as expected. The real problem here, which is easy to overlook, is that the String() method that implements the fmt.Stringer() interface will not be invoked when the object orange is being printed with fmt.Println() function, because the method String() is not being defined on a value but only on a pointer:

```
var orange Orange
orange.Increase(10)
orange.Decrease(5)
fmt.Println(orange)
// Output: {5}

orange := &Orange{}
orange.Increase(10)
orange.Decrease(5)
fmt.Println(orange)
// Output: 5
```

That is a subtle one, but the fix is simple. You need to redefine the String() method on a value instead of a pointer, and in that case, it will work for both pointers and values:

```
func (o Orange) String() string {
	return fmt.Sprintf("%v", o.Quantity)
}
```

## What might be wrong with the following small program?

```
func main() {
	scanner := bufio.NewScanner(strings.NewReader(`one
two
three
four
`))
	var (
		text string
		n    int
	)
	for scanner.Scan() {
		n++
		text += fmt.Sprintf("%d. %s\n", n, scanner.Text())
	}
	fmt.Print(text)

	// Output:
	// 1. One
	// 2. Two
	// 3. Three
	// 4. Four
}

```

The program numbers the lines in a buffer and uses the text/scanner to read the input line-by-line. What might be wrong with it?


Ans:

First, it is not necessary to collect the input in the string before putting it out to standard output. This example is slightly contrived.

Second, the string text is not modified with the += operator, it is created anew for every line. This is a significant difference between strings and []byte slices — strings in Go are non-modifiable. If you need to modify a string, use a []byte slice.

Here’s a provided small program, written in a better way:
```
func main() {
	scanner := bufio.NewScanner(strings.NewReader(`one
two
three
four
`))
	var (
		text []byte
		n    int
	)
	for scanner.Scan() {
		n++
		text = append(text, fmt.Sprintf("%d. %s\n", n, scanner.Text())...)
	}
	os.Stdout.Write(text)
	// 1. One
	// 2. Two
	// 3. Three
	// 4. Four
}
```

That is the point of the existence of both bytes and strings packages.

## What is the difference, if any, in the following two slice declarations, and which one is more preferable?

```
var a []int
```

and

```
a := []int{}
```


Ans: The first declaration does not allocate memory if the slice is not used, so this declaration method is preferred.

## Do you need both GOPATH and GOROOT variables, and why?

Most of the time, you do not need them both. You need only the GOPATH variable set pointing to the Go packages tree or trees.

GOROOT points to the root of the Go language home directory, but it is most probably already set to the directory of the current Go language installation. It is easy to check whether it is so with the go env command:

```
$ go env
…
GOROOT=“/home/zabb/go”
…
```

It is necessary to set the GOROOT variable if there are multiple Go language versions on the same system or if the Go language has been downloaded as a binary package taken from the internet or transferred from another system.


## What is GraphQL?

GraphQL is a query language created by Facebook in 2012 which provides a common interface between the client and the server for data fetching and manipulations.
The client asks for various data from the GraphQL server via queries. The response format is described in the query and defined by the client instead of the server: they are called client‐specified queries.
The structure of the data is not hardcoded as in traditional REST APIs — this makes retrieving data from the server more efficient for the client.

## List the key concepts of the GraphQL query language

* Key concepts of the GraphQL query language are:
* Hierarchical
* Product‐centric
* Strong‐typing
* Client‐specified queries
* Introspective

## Explain the main difference between REST and GraphQL

The main and most important difference between REST and GraphQL is that GraphQL is not dealing with dedicated resources, instead everything is regarded as a graph and therefore is connected and can be queried to app exact needs.

## How to do Server-side Caching? Or, what is a common challenge facing GraphQL.

One common concern with GraphQL, especially when comparing it to REST, are the difficulties to maintain server-side cache. With REST, it’s easy to cache the data for each endpoint, since it’s sure that the structure of the data will not change.

With GraphQL on the other hand, it’s not clear what a client will request next, so putting a caching layer right behind the API doesn’t make a lot of sense.
Server-side caching still is a challenge with GraphQL.

## Are there any disadvantages to GraphQL?


Disadvantages:

* You need to learn how to set up GraphQL. The ecosystem is still rapidly evolving so you have to keep up.
* You need to send the queries from the client, you can just send strings but if you want more comfort and caching you’ll use a client library -> extra code in your client
* You need to define the schema beforehand => extra work before you get results
* You need to have a graphql endpoint on your server => new libraries that you don’t know yet
* Graphql queries are more bytes than simply going to a REST endpoint
* The server needs to do more processing to parse the query and verify the parameters

## what is GraphQL Schema?

Every GraphQL server has two core parts that determine how it works: a schema and resolve functions.

The schema is a model of the data that can be fetched through the GraphQL server. It defines what queries clients are allowed to make, what types of data can be fetched from the server, and what the relationships between these types are.

Consider:

```
type Author {
  id: Int
  name: String
  posts: [Post]
}
type Post {
  id: Int
  title: String
  text: String
  author: Author
}
type Query {
  getAuthor(id: Int): Author
  getPostsByTitle(titleContains: String): [Post]
}
schema {
  query: Query
}
```

## Is GraphQL a Database Technology?
No. GraphQL is often confused with being a database technology. This is a misconception, GraphQL is a query language for APIs - not databases. In that sense it’s database agnostic and can be used with any kind of database or even no database at all.





## Hadoop questions

### What are some of the important features of Hadoop?

* Open Source: Hadoop represents an open source type framework which is to say that it is available free of charge. The users may also be allowed to alter the source code according to the requirements.
* Distributed processing: Hadoop supports the distributed processing of data whereby there is faster processing. The data within Hadoop HDFS is stored in a distributed fashion and MapReduce is obligated to the parallel processing of the that data.
* Fault tolerance: Hadoop itself is highly tolerant. It allows for the creation of three replicas for each of the blocks at different nodes by default. This number may be altered depending on the particular requirements. Therefore, it is possible to change this according to the requirements. It is possible to recover the data from another node in the event that one of the nodes is not successful. The particular detection of the node failure and the recovery of data is done automatically.
* Scalability: the other significant feature of Hadoop would is scalability. It is compatible with the many types of hardware and it's easy to access that new hardware within particular infrastructure nodes.
* Reliability: Hadoop stores the data in the cluster in a reliable manner, which would be independent of all other operations. That means the data that is stored within the Hadoop environment is not be affected by the failings of the machine.
* High availability: the data is stored within Hadoop and becomes available to access even after the hardware failure. In the event of hardware failure, the data may even be accessed from other paths.

### How are files stored in Hadoop?  What are Blocks?  What is the size of a Block in Hadoop?

A large file in  HDFS is broken into different parts and each of them is stored on a different Block. By default, a Block has a 64 MB capacity within HDFS.

### What do Block Scanners  do in Hadoop?

 Block Scanner refers to a program which every Data node in HDFS runs periodically in order to verify the checksum of each block stored within the data node. The goal of the Block Scanner would be detecting the data corruption errors on the Data node.

### In Hadoop what are different Node types?  

NameNode and DataNode.

### What is a NameNode?  What does it do?


The NameNode refers to the central node of a HDFS system. It does not store any of the data from the Map-Reduce operations. Though, it has metadata, which has been stored within the HDFS DataNodes. NameNode has the directory tree for the files within the HDFS filesystem. With the use of this metadata, it ends up managing the data, which is stored in the different DataNodes.

### What may occur if NameNode crashes in the HDFS cluster?

There is a NameNode when it comes to the HDFS cluster. This particular node maintains the metadata concerning the DataNodes. Because there is usually only one NameNode, it would be the single point of failure for the HDFS cluster. When the NameNode comes to an end, the system may not be available. You may specify a secondary NameNode within the HDFS Cluster. The secondary NameNametakes the regular checkpoints of the filing system within HDFS. However, it is not the backup for NameNode. It can be used for recreating NameNode and restarting it in the event of a crash.

### Which are the two messages, which NameNode gets from DataNode within Hadoop?

There are two messages which are attained from every DataNode:

* Block Report: this is a listing of the data blocks hosted on the DataNode. The report may also be useful for the functioning of the NameNode. With this particular report, NameNode would get information about the data that is stored on a particular DataNode.
* Heartbeat: this message signals that DataNode is still alive. The periodic receipt of Heartbeat is quite significant for NameNode in order to ascertain whether or not to use NameNode or not.

### How does Indexing work when it comes to Hadoop.

Indexing in Hadoop works in two different levels:

* Index based on the File URL: in this scenario, the data may be indexed based according to the different files. When you search for data, the index is going to return the files that have the data.
* Index based according to InputSplit: In this scenario, the data may be indexed according to the locations where the input split is located.

### What are the types of configurations (or configuration files) when it comes to Hadoop?

* Core-site.xml: Hadoop core configuration settings such as the I/O settings, which are common for HDFS and MapReduce. It may use a hostname for a port.
* Mapred-site.xml: would specify a framework name for MapReduce through setting mapreduce.framework. name.
* Hdfs-site.xml: configuration file has HDFS daemons settings. There is also specification of the default block permission and replication checking on HDFS.
* Yarn-site.xml: configuration file specifies configuration settings for ResourceManager and NodeManager.

### How does inner-cluster data copying function work within Hadoop?

In Hadoop, there is a utility which is known as DistCP, or Distributed Copy and its task is to perform large intra-cluster copying of the data. this utility is based as well on MapReduce. It creates Map tasks for the files given as the input. After every copy using the Distributed Copy, it is recommended to run crosschecks in order to confirm there is no corruption and copy is complete.


### What is Apache HBase?
It is a column-oriented database which is used to store the sparse data sets. It is run on the top of Hadoop file distributed system. Apache HBase is a database that runs on a Hadoop cluster. Clients can access HBase data through either a native Java API or through a Thrift or REST gateway, making it accessible by any language. Some of the key properties of HBase include:

* NoSQL: HBase is not a traditional relational database (RDBMS). HBase relaxes the ACID (Atomicity, Consistency, Isolation, Durability) properties of traditional RDBMS systems in order to achieve much greater scalability. Data stored in HBase also does not need to fit into a rigid schema like with an RDBMS, making it ideal for storing unstructured or semi-structured data.
* Wide-Column: HBase stores data in a table-like format with the ability to store billions of rows with millions of columns. Columns can be grouped together in “column families” which allows physical distribution of row values onto different cluster nodes.
* Distributed and Scalable: HBase group rows into “regions” which define how table data is split over multiple nodes in a cluster. If a region gets too large, it is automatically split to share the load across more servers.
* Consistent: HBase is architected to have “strongly-consistent” reads and writes, as opposed to other NoSQL databases that are “eventually consistent”. This means that once a write has been performed, all read requests for that data will return the same value.

### What is the reason of using HBase?
HBase is used because it provides random read and write operations and it can perform a number of operation per second on a large data sets.

### Define the difference between hive and HBase?
HBase is used to support record level operations but hive does not support record level operations.

### Define column families?
It is a collection of columns whereas row is a collection of column families.

### What is decorating Filters?
It is useful to modify, or extend, the behavior of a filter to gain additional control over the returned data.

### Define MapReduce.
MapReduce as a process was designed to solve the problem of processing in excess of terabytes of data in a scalable way.

Referred as the core of Hadoop, MapReduce is a programming framework to process large sets of data or big data across thousands of servers in a Hadoop Cluster. The concept of MapReduce is similar to the cluster scale-out data processing systems. The term MapReduce refers to two important processes of Hadoop program operates.

First is the map() job, which converts a set of data into another breaking down individual elements into key/value pairs (tuples). Then comes reduce() job into play, wherein the output from the map, i.e. the tuples serve as the input and are combined into smaller set of tuples. As the name suggests, the map job every time occurs before the reduce one.

### Illustrate a simple example of the working of MapReduce.
Let’s take a simple example to understand the functioning of MapReduce. However, in real-time projects and applications, this is going to be elaborate and complex as the data we deal with Hadoop and MapReduce is extensive and massive.

Assume you have five files and each file consists of two key/value pairs as in two columns in each file – a city name and its temperature recorded. Here, name of city is the key and the temperature is value.

```
San Francisco, 22
Los Angeles, 15
Vancouver, 30
London, 25
Los Angeles, 16
Vancouver, 28
London,12
```

It is important to note that each file may consist of the data for same city multiple times. Now, out of this data, we need to calculate the maximum temperature for each city across these five files. As explained, the MapReduce framework will divide it into five map tasks and each map task will perform data functions on one of the five files and returns maxim temperature for each city.


```
(San Francisco, 22)(Los Angeles, 16)(Vancouver, 30)(London, 25)
Similarly each mapper performs it for the other four files and produce intermediate results, for instance like below.

(San Francisco, 32)(Los Angeles, 2)(Vancouver, 8)(London, 27)
(San Francisco, 29)(Los Angeles, 19)(Vancouver, 28)(London, 12)
(San Francisco, 18)(Los Angeles, 24)(Vancouver, 36)(London, 10)
(San Francisco, 30)(Los Angeles, 11)(Vancouver, 12)(London, 5)

These tasks are then passed to the reduce job, where the input from all files are combined to output a single value. The final results here would be:

(San Francisco, 32)(Los Angeles, 24)(Vancouver, 36)(London, 27)
```

These calculations are perform instantly and are extremely efficient to calculate outputs on a large dataset.

### What is Shuffling and Sorting in MapReduce?
Shuffling and Sorting are two major processes operating simultaneously during the working of mapper and reducer.

The process of transferring data from Mapper to reducer is Shuffling. It is a mandatory operation for reducers to proceed their jobs further as the shuffling process serves as input for the reduce tasks.

In MapReduce, the output key-value pairs between the map and reduce phases (after the mapper) are automatically sorted before moving to the Reducer. This feature is helpful in programs where you need sorting at some stages. It also saves the programmer’s overall time.

### What is Partitioner and its usage?
Partitioner is yet another important phase that controls the partitioning of the intermediate map-reduce output keys using a hash function. The process of partitioning determines in what reducer, a key-value pair (of the map output) is sent. The number of partitions is equal to the total number of reduce jobs for the process.

Hash Partitioner is the default class available in Hadoop , which implements the following function.int getPartition(K key, V value, int numReduceTasks)
The function returns the partition number using the numReduceTasks is the number of fixed reducers.

### What is Identity Mapper and Chain Mapper?
Identity Mapper is the default Mapper class provided by Hadoop. when no other Mapper class is defined, Identify will be executed. It only writes the input data into output and do not perform and computations and calculations on the input data.

The class name is org.apache.hadoop.mapred.lib.IdentityMapper.

Chain Mapper is the implementation of simple Mapper class through chain operations across a set of Mapper classes, within a single map task. In this, the output from the first mapper becomes the input for second mapper and second mapper’s output the input for third mapper and so on until the last mapper.

### What are the key differences between Pig vs MapReduce?
PIG is a data flow language, the key focus of Pig is manage the flow of data from input source to output store. As part of managing this data flow it moves data feeding it to

process 1. taking output and feeding it to

process2. The core features are preventing execution of subsequent stages if previous stage fails, manages temporary storage of data and most importantly compresses and rearranges processing steps for faster processing. While this can be done for any kind of processing tasks Pig is written specifically for managing data flow of Map reduce type of jobs. Most if not all jobs in a Pig are map reduce jobs or data movement jobs. Pig allows for custom functions to be added which can be used for processing in Pig, some default ones are like ordering, grouping, distinct, count etc.

Mapreduce on the other hand is a data processing paradigm, it is a framework for application developers to write code in so that its easily scaled to PB of tasks, this creates a separation between the developer that writes the application vs the developer that scales the application. Not all applications can be migrated to Map reduce but good few can be including complex ones like k-means to simple ones like counting uniques in a dataset.

### What is partitioning?
Partitioning is a process to identify the reducer instance which would be used to supply the mappers output. Before mapper emits the data (Key Value) pair to reducer, mapper identify the reducer as an recipient of mapper output. All the key, no matter which mapper has generated this, must lie with same reducer.

### What is Google Cloud Dataproc?
Cloud Dataproc is Google Cloud Platform's fully-managed Apache Spark and Apache Hadoop service. Cloud Dataproc easily integrates with other GCP services, giving you a powerful and complete platform for data processing, analytics and machine learning.

### What are the operational commands of HBase?
Operational commands of HBase are Get, Delete, Put, Increment, and Scan.

### What is the use of ZooKeeper?
The zookeeper is used to maintain the configuration information and communication between region servers and clients. It also provides distributed synchronization.

### What is the  distributed consensus algorithm used in Zookeeper? What are alternatives?

Zookeeper uses ZAB.  Others are Paxos and Raft.  
Here is an article comparing them: https://www.alibabacloud.com/blog/a-brief-analysis-of-consensus-protocol-from-logical-clock-to-raft_594675


### Define compaction in HBase?
Compaction is a process which is used to merge the Hfiles into the one file and after the merging file is created and then old file is deleted. There are different types of tombstone markers which make cells invisible and these tombstone markers are deleted during compaction.

### Compare HBase with Hive?
Hive can help the SQL savvy to run MapReduce jobs. Since its JDBC compliant, it also integrates with existing SQL-based tools. Running Hive queries could take a while since they go over all of the data in the table by default. Nonetheless, the amount of data can be limited via Hive’s partitioning feature. Partitioning allows running a filter query over data that is stored in separate folders, and only read the data which matches the query. It could be used, for example, to only process files created between certain dates, if the files include the date format as part of their name.

HBase works by storing data as key/value. It supports four primary operations: put to add or update rows, scan to retrieve a range of cells, get to return cells for a specified row, and delete to remove rows, columns or column versions from the table. Versioning is available so that previous values of the data can be fetched (the history can be deleted every now and then to clear space via HBase compactions). Although HBase includes tables, a schema is only required for tables and column families, but not for columns, and it includes increment/counter functionality.

Hive and HBase are two different Hadoop-based technologies – Hive is an SQL-like engine that runs MapReduce jobs, and HBase is a NoSQL key/value database on Hadoop. But hey, why not use them both? Just like Google can be used for search and Facebook for social networking, Hive can be used for analytical queries while HBase for real-time querying. Data can even be read and written from Hive to HBase and back again.

 
### Compare HBase with Cassandra?
Both Cassandra and HBase are NoSQL databases, a term for which you can find numerous definitions. Generally, it means you cannot manipulate the database with SQL. However, Cassandra has implemented CQL (Cassandra Query Language), the syntax of which is obviously modeled after SQL.

Both are designed to manage extremely large data sets. HBase documentation proclaims that an HBase database should have hundreds of millions or — even better — billions of rows. Anything less, and you’re advised to stick with an RDBMS.
Both are distributed databases, not only in how data is stored but also in how the data can be accessed. Clients can connect to any node in the cluster and access any data.

In both Cassandra and HBase, the primary index is the row key, but data is stored on disk such that column family members are kept in close proximity to one another. It is, therefore, important to carefully plan the organization of column families. To keep query performance high, columns with similar access patterns should be placed in the same column family. Cassandra lets you create additional, secondary indexes on column values. This can improve data access in columns whose values have a high level of repetition — such as a column that stores the state field of a customer’s mailing address.

HBase lacks built-in support for secondary indexes but offers a number of mechanisms that provide secondary index functionality. 

### additional questions

https://www.edureka.co/blog/interview-questions/top-50-hadoop-interview-questions-2016/

https://intellipaat.com/blog/interview-question/big-data-hadoop-interview-questions/

https://www.tutorialspoint.com/hadoop/hadoop_interview_questions.htm

## What is Kafka?
Wikipedia defines Kafka as “an open-source message broker project developed by the Apache Software Foundation written in Scala and is a distributed publish-subscribe messaging system.

Feature	| Description
--- | ---
High Throughput	| Support for millions of messages with modest hardware
Scalability	| Highly scalable distributed systems with no downtime
Replication |	Messages are replicated across the cluster to provide support for multiple subscribers and balances the consumers in case of failures
Durability |	Provides support for persistence of message to disk
Stream Processing	| Used with real-time streaming applications like Apache Spark & Storm
Data Loss	| Kafka with proper configurations can ensure zero data loss


## List the various components in Kafka.
The four major components of Kafka are:

```
Topic – a stream of messages belonging to the same type
Producer – that can publish messages to a topic
Brokers – a set of servers where the publishes messages are stored
Consumer – that subscribes to various topics and pulls data from the brokers.
```

## Explain the role of the offset.
Messages contained in the partitions are assigned a unique ID number that is called the offset. The role of the offset is to uniquely identify every message within the partition.

## What is a Consumer Group?
Consumer Groups is a concept exclusive to Kafka.  Every Kafka consumer group consists of one or more consumers that jointly consume a set of subscribed topics.


## What is the role of the ZooKeeper?
Kafka uses Zookeeper to store offsets of messages consumed for a specific topic and partition by a specific Consumer Group.

## Is it possible to use Kafka without ZooKeeper?
No, it is not possible to bypass Zookeeper and connect directly to the Kafka server. If, for some reason, ZooKeeper is down, you cannot service any client request.

## Explain the concept of Leader and Follower.
Every partition in Kafka has one server which plays the role of a Leader, and none or more servers that act as Followers. The Leader performs the task of all read and write requests for the partition, while the role of the Followers is to passively replicate the leader. In the event of the Leader failing, one of the Followers will take on the role of the Leader. This ensures load balancing of the server.

## What roles do Replicas and the ISR play?
Replicas are essentially a list of nodes that replicate the log for a particular partition irrespective of whether they play the role of the Leader. On the other hand, ISR stands for In-Sync Replicas. It is essentially a set of message replicas that are synced to the leaders.

## Why are Replications critical in Kafka?
Replication ensures that published messages are not lost and can be consumed in the event of any machine error, program error or frequent software upgrades.

## If a Replica stays out of the ISR for a long time, what does it signify?
It means that the Follower is unable to fetch data as fast as data accumulated by the Leader.

## What is the process for starting a Kafka server?
Since Kafka uses ZooKeeper, it is essential to initialize the ZooKeeper server, and then fire up the Kafka server.

To start the ZooKeeper server: 
  > bin/zookeeper-server-start.sh config/zookeeper.properties

Next, to start the Kafka server: 
  > bin/kafka-server-start.sh config/server.properties

## How do you define a Partitioning Key?
Within the Producer, the role of a Partitioning Key is to indicate the destination partition of the message. By default, a hashing-based Partitioner is used to determine the partition ID given the key. Alternatively, users can also use customized Partitions.

## In the Producer, when does QueueFullException occur?
QueueFullException typically occurs when the Producer attempts to send messages at a pace that the Broker cannot handle. Since the Producer doesn’t block, users will need to add enough brokers to collaboratively handle the increased load.

## Explain the role of the Kafka Producer API.
The role of Kafka’s Producer API is to wrap the two producers – kafka.producer.SyncProducer and the kafka.producer.async.AsyncProducer. The goal is to expose all the producer functionality through a single API to the client.

## What is the main difference between Kafka and Flume?
Even though both are used for real-time processing, Kafka is scalable and ensures message durability.

## What are different types of ML?

* supervised

It is like learning under the guidance of a teacher
Training dataset is like a teacher which is used to train the machine
Model is trained on a pre-defined dataset before it starts making decisions when given new data

* unsupervised

It is like learning without a teacher.
Model learns through observation & finds structures in data.
Model is given a dataset and is left to automatically find patterns and relationships in that dataset by creating clusters.

* reinforcement

It is like being stuck in an isolated island, where you must explore the environment and learn how to live and adapt to the living conditions on your own.
Model learns through the hit and trial method
It learns on the basis of reward or penalty given for every action it performs


## How does deep learning differ from ML?

deep learning is a form of machine learning that is inspired by the structure of the brain and is particularly effective in feature detection.

ML is all about algorithms that parse data, learn from that data, and then apply what they've learned to make informed decisions.

## Explain classification and regression

classification | regression
--- | ---
task of predicting a discrete class label | predicting a continuous quantity
data is labelled into one of two more classes | requires prediction of a quantity
binary or multi-class classification | problems with multiple input variables is called multivariate regression program
classifying an email as spam or non spam is an example | predicting the price of a stock over a period of time is an example


## What is selection bias?

* statistical error that causes a bias in the sampling portion of an experiment
* error causes one smapling group to be selected more often than the other groups
* selection bias may produce an inaccurate conclusion if the selection bias is not identified

## what is precision and recall?

example:

Imagine that, your girlfriend gave you a birthday surprise every year for the last 10 years. One day, your girlfriend asks you: ‘Sweetie, do you remember all the birthday surprises from me?’
To stay on good terms with your girlfriend, you need to recall all the 10 events from your memory. Therefore, recall is the ratio of the number of events you can correctly recall, to the total number of events.
If you can recall all 10 events correctly, then, your recall ratio is 1.0 (100%) and if you can recall 7 events correctly, your recall ratio is 0.7 (70%)
However, you might be wrong in some answers.

For example, let’s assume that you took 15 guesses out of which 10 were correct and 5 were wrong. This means that you can recall all events but not so precisely
Therefore, precision is the ratio of a number of events you can correctly recall, to the total number of events you can recall (mix of correct and wrong recalls).
From the above example (10 real events, 15 answers: 10 correct, 5 wrong), you get 100% recall but your precision is only 66.67% (10 / 15)

## what is confusion matrix?

A confusion matrix or an error matrix is a table which is used for summarizing the performance of a classification algorithm. 

## What is the difference between inductive and deductive learning?
Inductive learning is the process of using observations to draw conclusions 
Deductive learning is the process of using conclusions to form observations 

## How is KNN different from K-means clustering?

K-Nearest neighbor | K-Means clustering
--- | ---
Supervised | Unsupervised
Used for classification or regression | used for clustering
K in KNN represents the number of nearest neighbors used to classify or predict in case of continuous variable | K in K-means represents the number of clusters the algorithm is trying to identify or learn from data


##  Is it better to have too many false positives or too many false negatives? Explain.

It depends on the question as well as on the domain for which we are trying to solve the problem. If you’re using Machine Learning in the domain of medical testing, then a false negative is very risky, since the report will not show any health problem when a person is actually unwell. Similarly, if Machine Learning is used in spam detection, then a false positive is very risky because the algorithm may classify an important email as spam.

## What is the difference between Gini Impurity and Entropy in a Decision Tree?
Gini Impurity and Entropy are the metrics used for deciding how to split a Decision Tree.
Gini measurement is the probability of a random sample being classified correctly if you randomly pick a label according to the distribution in the branch.
Entropy is a measurement to calculate the lack of information. You calculate the Information Gain (difference in entropies) by making a split. This measure helps to reduce the uncertainty about the output label.

## What is the difference between Entropy and Information Gain?
Entropy is an indicator of how messy your data is. It decreases as you reach closer to the leaf node.
The Information Gain is based on the decrease in entropy after a dataset is split on an attribute. It keeps on increasing as you reach closer to the leaf node.


## What is Overfitting? And how do you ensure you’re not overfitting with a model?
Over-fitting occurs when a model studies the training data to such an extent that it negatively influences the performance of the model on new data.

This means that the disturbance in the training data is recorded and learned as concepts by the model. But the problem here is that these concepts do not apply to the testing data and negatively impact the model’s ability to classify the new data, hence reducing the accuracy on the testing data.

Three main methods to avoid overfitting:

Collect more data so that the model can be trained with varied samples.
Use ensembling methods, such as Random Forest. It is based on the idea of bagging, which is used to reduce the variation in the predictions by combining the result of multiple Decision trees on different samples of the data set.
Choose the right algorithm.

## How would you screen for outliers and what should you do if you find one?
The following methods can be used to screen outliers:

* Boxplot: A box plot represents the distribution of the data and its variability. The box plot contains the upper and lower quartiles, so the box basically spans the Inter-Quartile Range (IQR). One of the main reasons why box plots are used is to detect outliers in the data. Since the box plot spans the IQR, it detects the data points that lie outside this range. These data points are nothing but outliers.
* Probabilistic and statistical models: Statistical models such as normal distribution and exponential distribution can be used to detect any variations in the distribution of data points. If any data point is found outside the distribution range, it is rendered as an outlier.
* Linear models: Linear models such as logistic regression can be trained to flag outliers. In this manner, the model picks up the next outlier it sees.
* Proximity-based models: An example of this kind of model is the K-means clustering model wherein, data points form multiple or ‘k’ number of clusters based on features such as similarity or distance. Since similar data points form clusters, the outliers also form their own cluster. In this way, proximity-based models can easily help detect outliers.
How do you handle these outliers?

If your data set is huge and rich then you can risk dropping the outliers.
However, if your data set is small then you can cap the outliers, by setting a threshold percentile. For example, the data points that are above the 95th percentile can be used to cap the outliers.
Lastly, based on the data exploration stage, you can narrow down some rules and impute the outliers based on those business rules.

##  What is bagging and boosting in Machine Learning?

Similarities | Difference
---- | ----
both are ensemble methods to get N learns from 1 learner | boosting tries to add new models that do well where previous models fail
both generate several training data sets by random sampling | only boosting determines weight for the data to tip the scales in favour of the most difficult cases
both make final decision by taking the average of N learners | bagging uses equal average and boosting uses weighted average
both are good at reducing variance and proving higher scalability | only boosting tries to reduce bias.  Bagging may solve the problem of overfitting. Boosting may increase overfit.

https://quantdare.com/what-is-the-difference-between-bagging-and-boosting/

## What are collinearity and multicollinearity?
* Collinearity occurs when two predictor variables (e.g., x1 and x2) in a multiple regression have some correlation.
* Multicollinearity occurs when more than two predictor variables (e.g., x1, x2, and x3) are inter-correlated.


##  What do you understand by Eigenvectors and Eigenvalues?
* Eigenvectors: Eigenvectors are those vectors whose direction remains unchanged even when a linear transformation is performed on them.
* Eigenvalues: Eigenvalue is the scalar that is used for the transformation of an Eigenvector.

## What is A/B Testing?
A/B is Statistical hypothesis testing for randomized experiment with two variables A and B. 
It is used to compare two models that use different predictor variables in order to check which variable fits best for a given sample of data.
Consider a scenario where you’ve created two models (using different predictor variables) that can be used to recommend products for an e-commerce platform.
A/B Testing can be used to compare these two models to check which one best recommends products to a customer.

## What is Cluster Sampling?
It is a process of randomly selecting intact groups within a defined population, sharing similar characteristics.
Cluster Sample is a probability sample where each sampling unit is a collection or cluster of elements.
For example, if you’re clustering the total number of managers in a set of companies, in that case, managers (samples) will represent elements and companies will represent clusters.

## You are given a data set consisting of variables having more than 30% missing values? Let’s say, out of 50 variables, 8 variables have missing values higher than 30%. How will you deal with them?
Assign a unique category to the missing values, who knows the missing values might uncover some trend.
We can remove them blatantly.
Or, we can sensibly check their distribution with the target variable, and if found any pattern we’ll keep those missing values and assign them a new category while removing others.

## There’s a game where you are asked to roll two fair six-sided dice. If the sum of the values on the dice equals seven, then you win $21. However, you must pay $5 to play each time you roll both dice. Do you play this game? And in the follow-up: If he plays 6 times what is the probability of making money from this game?
* The first condition states that if the sum of the values on the 2 dices is equal to 7, then you win $21. But for all the other cases you must pay $5.
* First, let’s calculate the number of possible cases. Since we have two 6-sided dices, the total number of cases => 6*6 = 36.
* Out of 36 cases, we must calculate the number of cases that produces a sum of 7 (in such a way that the sum of the values on the 2 dices is equal to 7)
* Possible combinations that produce a sum of 7 is, (1,6), (2,5), (3,4), (4,3), (5,2) and (6,1). All these  6 combinations generate a sum of 7.
* This means that out of 36 chances, only 6 will produce a sum of 7. On taking the ratio, we get: 6/36 = 1/6
* So this suggests that we have a chance of winning $21, once in 6 games.
* So to answer the question if a person plays 6 times, he will win one game of $21, whereas for the other 5 games he will have to pay $5 each, which is $25 for all five games. Therefore, he will face a loss because he wins $21 but ends up paying $25.


## ‘People who bought this also bought…’ recommendations seen on Amazon is based on which algorithm?

E-commerce websites like Amazon make use of Machine Learning to recommend products to their customers. The basic idea of this kind of recommendation comes from collaborative filtering. Collaborative filtering is the process of comparing users with similar shopping behaviors in order to recommend products to a new user with similar shopping behavior.

To better understand this, let’s look at an example. Let’s say a user A who is a sports enthusiast bought, pizza, pasta, and a coke.  Now a couple of weeks later, another user B who rides a bicycle buys pizza and pasta. He does not buy the coke, but Amazon recommends a bottle of coke to user B since his shopping behaviors and his lifestyle is quite similar to user A. This is how collaborative filtering works.


## What is PCA? 

Principal components analysis (PCA, for short) is a variable-reduction technique that shares many similarities to exploratory factor analysis. Its aim is to reduce a larger set of variables into a smaller set of 'artificial' variables, called 'principal components', which account for most of the variance in the original variables.

There are a number of common uses for PCA: (a) you have measured many variables (e.g., 7-8 variables, represented as 7-8 questions/statements in a questionnaire) and you believe that some of the variables are measuring the same underlying construct (e.g., depression). If these variables are highly correlated, you might want to include only those variables in your measurement scale (e.g., your questionnaire) that you feel most closely represent the construct, removing the others; (b) you want to create a new measurement scale (e.g., a questionnaire), but are unsure whether all the variables you have included measure the construct you are interested in (e.g., depression). Therefore, you test whether the construct you are measuring 'loads' onto all (or just some) of your variables. This helps you understand whether some of the variables you have chosen are not sufficiently representative of the construct you are interested in, and should be removed from your new measurement scale; (c) you want to test whether an existing measurement scale (e.g., a questionnaire) can be shortened to include fewer items (e.g., questions/statements), perhaps because such items may be superfluous (i.e., more than one item may be measuring the same construct) and/or there may be the desire to create a measurement scale that is more likely to be completed (i.e., response rates tend to be higher in shorter questionnaires). These are just some of the common uses of PCA. It is also worth noting that whilst PCA is conceptually different to factor analysis, in practice it is often used interchangeably with factor analysis, and is included within the 'Factor procedure' in SPSS Statistics.

## You are given a data set. The data set contains many variables, some of which are highly correlated and you know about it. Your manager has asked you to run PCA. Would you remove correlated variables first? Why?
Possibly, you might get tempted to say no, but that would be incorrect.
Discarding correlated variables will have a substantial effect on PCA because, in the presence of correlated variables, the variance explained by a particular component gets inflated.

## What is Boosting?
Boosting refers to a group of algorithms which transforms weak learner to strong learners.
Boosting algorithms are classified into: 


* Gradient Boosting
* XGBoost
* AdaBoost etc.




## What is Gradient Boosting in Machine Learning: 
Gradient boosting is a machine learning technique for regression and classification problems which constructs a prediction model in the form of an ensemble of weak prediction models.

## What’s an ensemble?
It is simply a group of items viewed as a whole rather than individually.

A GBM basically creates lots of individual predictors and each of them tries to predict the true label. Then, it gives its final prediction by averaging all those individual predictions (note however that it is not a simple average but a weighted average).


## Difference betweeen random frest and GBM?  "Averaging the predictions made by lots of predictors”.. that sounds like Random Forest!

That is in fact what an ensemble method is. And random forests and gradient boosting machines are just 2 types of ensemble methods.
One important difference between the two is that the predictors used in Random forest are independent of each other whereas the ones used in gradient boosting machines are built sequentially where each one tries to improve upon the mistakes made by its predecessor.

There is another class of tree ensembles called — Random Forests. While GBMs are a type of boosting algorithm, this is a bagging algorithm . So, despite being implemented using decision trees like GBMs, Random Forests are much different from them. Random Forests are great because they will generally give you a good enough result with the default parameter settings, unlike XGBoost and LightGBM which require tuning. But once tuned, XGBoost and LightGBM are much more likely to perform better.

## how does the algorithm decide the number of predictors to put in the ensemble?

It does not. We do. And that brings us to our first important parameter — n_estimators : We pass the number of predictors that we want the GBM to build inside the n_estimators parameter. The default number is 100.
So, let’s talk about these individual predictors now.

In theory, these predictors can be any regressor or classifier but in practice, decision trees give the best results.

The sklearn API for LightGBM provides a parameter- boosting_type and the API for XGBoost has parameter- booster to change this predictor algorithm. You can choose from —  gbdt, dart, goss, rf (LightGBM) or gbtree, gblinear or dart (XGBoost). Note that a decision tree, almost always, outperforms the other options by a fairly large margin. The good thing is that it is the default setting for this parameter; so you don’t have to worry about it.

## Finding the best set of hyperparameters
You can use sklearn’s RandomizedSearchCV in order to find a good set of hyperparameters. It will randomly search through a subset of all possible combinations of the hyperparameters and return the best possible set of hyperparameters(or at least something close to the best).

But if you wish to go even further, you could look around the hyperparameter set that it returns using GridSearchCV. Grid search will train the model using every possible hyperparameter combination and return the best set. Note that since it tries every possible combination, it can be expensive to run.



##  Explain the working of decision trees and XGBoost and all the models(Bagging, Random Forest, Boosting, Gradient Boosting) in between. Talk about parallelization in these models. Talk about bias/variance for these models.
XGBoost is a decision-tree-based ensemble Machine Learning algorithm that uses a gradient boosting framework. In prediction problems involving unstructured data (images, text, etc.) artificial neural networks tend to outperform all other algorithms or frameworks. However, when it comes to small-to-medium structured/tabular data, decision tree based algorithms are considered best-in-class right now. 

![evolution of xgboost from decision trees](https://miro.medium.com/max/1400/1*QJZ6W-Pck_W7RlIDwUIN9Q.jpeg)

XGBoost algorithm was developed as a research project at the University of Washington. Tianqi Chen and Carlos Guestrin presented their paper at SIGKDD Conference in 2016 and caught the Machine Learning world by fire. Since its introduction, this algorithm has not only been credited with winning numerous Kaggle competitions but also for being the driving force under the hood for several cutting-edge industry applications. As a result, there is a strong community of data scientists contributing to the XGBoost open source projects with ~350 contributors and ~3,600 commits on GitHub. The algorithm differentiates itself in the following ways:
A wide range of applications: Can be used to solve regression, classification, ranking, and user-defined prediction problems.
Portability: Runs smoothly on Windows, Linux, and OS X.
Languages: Supports all major programming languages including C++, Python, R, Java, Scala, and Julia.
Cloud Integration: Supports AWS, Azure, and Yarn clusters and works well with Flink, Spark, and other ecosystems.

Imagine that you are a hiring manager interviewing several candidates with excellent qualifications. Each step of the evolution of tree-based algorithms can be viewed as a version of the interview process.

* Decision Tree: Every hiring manager has a set of criteria such as education level, number of years of experience, interview performance. A decision tree is analogous to a hiring manager interviewing candidates based on his or her own criteria.
* Bagging: Now imagine instead of a single interviewer, now there is an interview panel where each interviewer has a vote. Bagging or bootstrap aggregating involves combining inputs from all interviewers for the final decision through a democratic voting process.
* Random Forest: It is a bagging-based algorithm with a key difference wherein only a subset of features is selected at random. In other words, every interviewer will only test the interviewee on certain randomly selected qualifications (e.g. a technical interview for testing programming skills and a behavioral interview for evaluating non-technical skills).
* Boosting: This is an alternative approach where each interviewer alters the evaluation criteria based on feedback from the previous interviewer. This ‘boosts’ the efficiency of the interview process by deploying a more dynamic evaluation process.
* Gradient Boosting: A special case of boosting where errors are minimized by gradient descent algorithm e.g. the strategy consulting firms leverage by using case interviews to weed out less qualified candidates.
* XGBoost: Think of XGBoost as gradient boosting on ‘steroids’ (well it is called ‘Extreme Gradient Boosting’ for a reason!). It is a perfect combination of software and hardware optimization techniques to yield superior results using less computing resources in the shortest amount of time.

## Why does XGBoost perform so well?
XGBoost and Gradient Boosting Machines (GBMs) are both ensemble tree methods that apply the principle of boosting weak learners (CARTs generally) using the gradient descent architecture. However, XGBoost improves upon the base GBM framework through systems optimization and algorithmic enhancements.

System Optimization:

* Parallelization: XGBoost approaches the process of sequential tree building using parallelized implementation. This is possible due to the interchangeable nature of loops used for building base learners; the outer loop that enumerates the leaf nodes of a tree, and the second inner loop that calculates the features. This nesting of loops limits parallelization because without completing the inner loop (more computationally demanding of the two), the outer loop cannot be started. Therefore, to improve run time, the order of loops is interchanged using initialization through a global scan of all instances and sorting using parallel threads. This switch improves algorithmic performance by offsetting any parallelization overheads in computation.

* Tree Pruning: The stopping criterion for tree splitting within GBM framework is greedy in nature and depends on the negative loss criterion at the point of split. XGBoost uses ‘max_depth’ parameter as specified instead of criterion first, and starts pruning trees backward. This ‘depth-first’ approach improves computational performance significantly.

* Hardware Optimization: This algorithm has been designed to make efficient use of hardware resources. This is accomplished by cache awareness by allocating internal buffers in each thread to store gradient statistics. Further enhancements such as ‘out-of-core’ computing optimize available disk space while handling big data-frames that do not fit into memory.

Algorithmic Enhancements:

* Regularization: It penalizes more complex models through both LASSO (L1) and Ridge (L2) regularization to prevent overfitting.

* Sparsity Awareness: XGBoost naturally admits sparse features for inputs by automatically ‘learning’ best missing value depending on training loss and handles different types of sparsity patterns in the data more efficiently.

* Weighted Quantile Sketch: XGBoost employs the distributed weighted Quantile Sketch algorithm to effectively find the optimal split points among weighted datasets.

* Cross-validation: The algorithm comes with built-in cross-validation method at each iteration, taking away the need to explicitly program this search and to specify the exact number of boosting iterations required in a single run.


## So should we use just XGBoost all the time?

Picking the right algorithm is not enough. We must also choose the right configuration of the algorithm for a dataset by tuning the hyper-parameters.

Furthermore, there are several other considerations for choosing the winning algorithm such as :
  
  * computational complexity
  * explainability
  * ease of implementation
  
This is exactly the point where Machine Learning starts drifting away from science towards art -- that’s where the magic happens!

## Additional predictive modeling questions

https://github.com/JifuZhao/120-DS-Interview-Questions/blob/master/predictive-modeling.md


## What is Tensorflow?

TensorFlow is a machine learning library created by the Brain Team of Google and made open source in 2015. 

Basically, Tensorflow is a low-level toolkit for doing complicated math and it offers the 
users customizability to build experimental learning architectures, to work with them and to 
turn them into running software.



## What are Tensors?
Tensors are higher dimensional arrays which are used in computer programming to represent a multitude of 
data in the form of numbers. There are other n-d array libraries 
available on the internet like Numpy but TensorFlow 
stands apart from them as it offers methods to create 
tensor functions and automatically compute derivatives.

## What is a TensorBoard?
TensorBoard, a suit of visualizing tools, is an easy solution to Tensorflow offered by the creators that lets 
you visualize the graphs, plot quantitative metrics about the graph with additional 
data like images to pass through it.



## List a few advantages of TensorFlow?


* It has platform flexibility
* It is easily trainable on CPU as well as GPU for distributed computing.
* TensorFlow has auto differentiation capabilities
* It has advanced support for threads, asynchronous computation, and queue es.
* It is a customizable and open source.


## List a few limitations of Tensorflow.


* Has GPU memory conflicts with Theano if imported in the same scope.
* No support for OpenCL
* Requires prior knowledge of advanced calculus and linear algebra along with a pretty good understanding of machine learning.


## What are TensorFlow servables?

These are the central rudimentary units in TensorFlow Serving.  
Objects that clients use to perform the computation are called Servables.

The size of a servable is flexible. 
A single servable might include anything from a lookup table to a single model to a tuple of inference models. 



## What do the TensorFlow managers do?

Tensorflow Managers handle the full lifecycle of Servables, including:


* Loading Servables
* Serving Servables
* Unloading Servables



## What are TensorFlow loaders?

Tensorflow Loaders are used for adding algorithms and data backends one of which 
is tensorflow itself. For example, a loader can be implemented to load, 
access and unload a new type of servable machine learning model.

## What do you mean by sources in TensorFlow?

Sources are in simple terms, modules that find and provide servables. 
Each Source provides zero or more servable streams. One Loader is supplied 
for each servable version it makes available to be loaded.

## What are the APIs inside the TensorFlow project?

The API’s inside TensorFlow are still Python-based and they have low-level 
options for its users such as tf.manual or tf.nnrelu which use to build neural 
network architecture. These APIs also use to aid designing deep neural network 
having higher levels of abstraction.

## What are the APIs outside TensorFlow project?


* TFLearn: This API shouldn’t be seen as TF Learn, which is TensorFlow’s  tf.contrib.learn. It is a separate Python package.
* TensorLayer: It comes as a separate package and is different from what TensorFlow’s layers API has in its bag.
* Pretty Tensor: It is actually a Google project which offers a fluent interface with chaining.
* Sonnet: It is a project of Google’s DeepMind which features a modular approach.



## In TensorFlow, what exactly Bias and Variance are? Do you find any similarity between them?

In the learning algorithms, Biases can consider as errors which can result in failure of 
entire model and can alter the accuracy. Some experts believe these errors are essential to enable leaner’s 
gain knowledge from a training point of view.


## Can TensorFlow be deployed in container software?

Tensorflow can also use with containerization tools such as docker, for instance, 
it could use to deploy a sentiment analysis model which uses character level 
ConvNet networks for text classification. 

## What exactly Neural Networks are? What are the types of same you are familiar with?

Neural networks as the name suggests are a network of elemental processing entities 
that together make a complex form. There can be Artificial Neural Networks and
Biological Neural Networks. The use of artificial neural networks 
is more common as they try to imitate the mechanics of the human brain.



## What are the general advantages of using the Artifical Neural Networks?

They use to find answers to complex problems in a stepwise manner. All the information that 
a network can receive can easily be in any format. They also make use of 
real-time operations along with a good tolerance capability.

## What exactly do you know about Recall and Precision?

The other name of Recall is the true positive rate. It is the overall figure of 
positiveness a model can generally claim. The predictive value which is generally p
ositive in nature is Precision. The difference between the true positive rate and 
claimed positive rate can be defined with the help of both these options. 

## What difference do you find in Type I and Type II errors?

Type I error means a false positive value while Type II error means a false negative.

## What would be your strategy to handle a situation indicating an imbalanced dataset?

This usually occurs when a vast set of data keep in a single class. 
Sampling the dataset again is one of the possible solutions and the other one 
being the migration of data to parallel classes. The dataset should not be damaged. 

## What exactly do you know about Bias-Variance decomposition?

It generally uses to decompose problems such as errors that occur during learning in 
different algorithms. Bias keeps reducing if the data is to be made complex. Trading off the 
Variance and Bias are very essential to get results that are totally free from errors. 

## What are word embeddings used for and can they be used in TensorFlow?

Word embeddings usually use in Natural Language Processing as a representation of 
words and they can use in TensorFlow where it also call as word2vec.

## What is the MNIST dataset?

It is a dataset containing information of handwritten digits.

## What are Bayesian Statistics and Bayes Theorem?


It calculates the degree of belief in a certain event and gives a probability 
of the occurrence of some statistical problem.

Let’s consider an example:

```
Suppose, from 4 basketball matches, John won 3 and Harry won only one.
Now, if you have to bet on either John or Harry. So, what would you do?
The answer is obvious – John.

But, let’s add another factor to the match, which is rain. When Harry won, it was raining. But, when John won, out of 3 matches, 1 time it was raining.
If the weather forecast says that there is an extremely high possibility of rain on the day of the next match. So, who would you bet on?
Even without using it, you can tell that the comparison basis has changed and chances of Harry winning have increased.
```

That is where Bayesian statistics  helps. Hence, the exact probability can be calculated with Bayes theorem.

The Bayes theorem is:

```
P (A/B) = P(B/A)P(A) / P(B)
```

Considering the above example, here’s what the values are:
```
       P(A) = ¼, Harry won one out of 4 matches.
       P(B) = ½, it rained two times out of 4 match days.
       P(B/A) = 1, when Harry won it was raining.
```
Placing the values in the formula, the chances of Harry winning will become 50%, which was only 25% earlier.

## How is Bayesian useful in ML?  Or is ML different than Bayesian statistics?

Machine learning simply tries to predict something about a certain system based on data available. 
But Bayesian statistics, on the other hand, is the degree of belief.

Bayesian machine learning is useful when there are fewer data available. 
So, using this method, it is predicted what the model will look like based on prior knowledge.

For instance, predicting whether a coin will land on tails lead to uncertainty. 
The scope of the answer will be limited. 

If you flip this coin 100 times and receive 50 tails and 50 heads, then you can say the probability is 50%. 
But, what if the result is 70 times tails and 30 times heads?

We all know the probability of heads and tails while flipping a coin is 50-50. 
With less data, you have the chances of landing on an incorrect conclusion.

Baye’s theorem is useful for determining the probability of an event, obtained by 
dividing the actual positive rate by the false positive rate. 
Some of the very complex questions and challenges can solve using a 
simple approach and eliminated with the help of this theorem.


### What are three naive Bayes classifiers?

There are three naïve Bayes classifiers:


* The Multinomial classifier uses multinomial distribution on each word of a sentence. Every word is treated independently rather than being treated as a part of the sentence.
* The Gaussian classifier is utilized with continuous data. It assumes that each data class is distributed as a Gaussian distribution.
* The Bernoulli classifier assumes that every feature present is binary, which means it can only take either of the two values.


## What is MQTT in IoT?
MQTT is the standard protocol for messaging and data exchange for the Internet of Things. The protocol uses a publish/subscribe architecture. The technology provides a scalable and cost-effective way to connect devices over the Internet. It is able to deliver data over the Internet in near real-time and with guarantees of delivery. MQTT is designed for IoT devices - lightweight, which enables low-cost device communication.

## Who uses MQTT?
MQTT is used by many major companies, especially in the automotive, industry 4.0, transport, and entertainment sectors. MQTT is used for data exchange between constrained devices and server applications. It keeps bandwidth requirements to an absolute minimum, handles unreliable networks, requires little implementation effort for developers, and is, therefore, ideal for machine-to-machine (M2M) communication.

## How does MQTT work?
MQTT follows the Publish/Subscribe paradigm. The sender (Publisher) and receiver (Subscribers) of messages communicate via so-called topics and are decoupled from each other. The connection between them is handled by the broker. The task of the broker is to filter all incoming messages and distribute them correctly to the subscribers. A client doesn’t have to pull the information it needs, the broker pushes the information to the client whenever something new is available.

## What is an MQTT client?
An MQTT client is any device (from a microcontroller to a full-fledged server) that operates an MQTT library and connects to an MQTT broker over a network. Each MQTT client can be both publisher and/or subscriber.

## What does an MQTT broker do?
An MQTT broker is at the heart of any MQTT deployment. Depending on the implementation, a broker can handle up to millions of concurrently connected MQTT clients. The broker is responsible for receiving all messages, filtering the messages, determining who is interested in each message, and sending the message to these subscribed clients.

## What is an MQTT topic?
Communication in MQTT is based on the topic principle. An MQTT topic is a UTF-8 string that the broker uses to filter messages for each connected client. To receive messages, the client must subscribe to the topic. A topic can have one or more topic levels. Each topic level is separated by a slash (Topic Level Separator).

## Is MQTT secure?
MQTT is designed to allow very secure communication. As an application layer protocol it introduces extensive device authentication and authorization possibilities. The underlying TCP/IP transport protocol can add additional security via TLS encryption.

## Is MQTT open source?
MQTT is an open protocol that is standardized by OASIS and ISO (ISO/IEC 20922:2016).

## What is the difference between HTTP and MQTT?
MQTT is a data-centric, extremely lightweight, binary protocol. Due to its minimal packet overhead, MQTT excels when transferring data over the wire in comparison to document-centric protocols such as HTTP. Unlike HTTP, which is based on a request/response pattern, MQTT provides push-based communication. This push is made possible via standing TCP connections.

## What is the difference between AMQP and MQTT?
AMQP is bi-directional, synchronous peer-to-peer messaging protocol that has high demands for implementation complexity and a larger network overhead. It is a binary wire protocol, build as replacement for message middleware with main focus on interoperability between different vendors via rich featuring and several exchange patterns.

## MQTT is a binary protocol with strength in simplicity to be ideal for mobile IoT app and M2M. It provides the pub/sub messaging pattern and is designed for resource-constrained devices, low bandwidth and high latency networks. MQTT is specified by the official OASIS Standard.

## Does MQTT use WebSockets?
With the right broker implementation that supports native WebSockets, MQTT with 100% of its features set can be used via WebSockets. As they provide a bi-directional, ordered, and lossless communication channel via TCP.

## Does MQTT use TCP or UDP?
MQTT uses TCP. Due to ordering requirements MQTT over UDP is not possible.

## Does MQTT require internet?
Yes, to send or receive messages, the MQTT client must establish a TCP connection to the broker. However, MQTT comes with features specifically designed to cope with unstable network connections, like the broker buffering incoming messages for disconnected clients.

## Does MQTT work with Apache Kafka?
Yes, MQTT and Kafka can be integrated with one another. The most efficient way to do so is to use the HiveMQ Enterprise Kafka Extension.

## Is MQTT restful?
No. MQTT is not stateless and does not provide a request/response pattern. It is a publish/subscribe application layer messaging protocol that requires a standing TCP connection and transmit messages in an instantaneous, push way.


## What are some NoSQL databases?  Please list and describe them

## What are some types of NoSQL databases?

* Key Value Store type database
* Document Store type database
* Column STore type database
* Graph Database

##  Can you describe which NoSQL database is which type?


## What are some NoSQL database features?

* Schema Agnostic
* AutoSharding and Elasticity
* Highly Distributable
* Easily Scalable
* Integrated Caching


## Give the name of some components of Cassandra and explain each.

Some components of Cassandra are:

* Table
* Node
* Cluster
* Data Centre
* Memtable
* SSTable
* Commit log
* Bloom Filter

## Tell something about the query language used in Cassandra Database.

Cassandra query language is used for Cassandra Database. It is an interface that a user uses to access the database. It basically is a communication medium. All the operations are carried out from this panel.

## Define commit log.

It is a mechanism that is used to recover data in case the database crashes. Every operation that is carried out is saved in the commit log. Using this the data can be recovered.

## Name the types of tunable consistency.

Cassandra support two types of consistencies:

* Eventual Consistency

* Strong Consistency


## Define SSTable.

 SSTable is Sorted String Table. It is a data file that accepts regular Mem Tables.

## Describe Memtable.

 Memtables are basically a cache space containing content in key and column format.


## Give a list of Collection data type in Cassandra.

 There are three type of collection data type:

* Set
* List
* Map

## What is MongoDB?
MongoDB (from humongous) is a cross-platform document-oriented database. Classified as a NoSQL database, MongoDB eschews the traditional table-based relational database structure in favor of JSON-like documents with dynamic schemas (MongoDB calls the format ‘BSON’), making the integration of data in certain types of applications easier and faster. Released under a combination of the GNU Affero General Public License and the Apache License, MongoDB is open-source.

MongoDB was first developed by the software company 10gen (now, MongoDB Inc.) in October 2007 as a component of a planned platform as a service product. Then, the company shifted to an open-source development model in 2009, with 10gen offering commercial support and other services. Since then, MongoDB has been adopted as backend software by a number of major websites and services, including Craigslist, eBay, Foursquare, SourceForge, Viacom, and the New York Times, among others. Currently, MongoDB is the most popular NoSQL database system.

## What do you understand by NoSQL databases? Is MongoDB a NoSQL database? Explain.
Presently, the Internet is loaded with big data, big users, and so on that are becoming more complex day by day. NoSQL is the answer to all these problems; it is not a traditional database management system, not even a relational database management system (RDBMS).
NoSQL stands for ‘Not only SQL’, and it is a type of database that can handle and sort all types of unstructured, messy, and complicated data. It is just a new way to think about databases. MongoDB is a NoSQL database.


## What is the difference between MongoDB and MySQL?
Although both MongoDB and MySQL are free and open-source databases, there is a lot of difference between them in terms of data representation, relationships, transaction, querying data, schema design and definition, performance speed, normalization, and many more. To compare MySQL with MongoDB is like a comparison between relational and non-relational databases.

## What are mongoDB features?

* Document-oriented (DO)
* High performance (HP)
* High availability (HA)
* Easy scalability
* Rich query language

## When and to what extent does data get extended to multi-slice?
MongoDB scrap stands on a collection. So, an album of all substances is kept in a lump or mass. Only when there is an additional time slot, there will be more than a few slice data achievement choices, but when there is more than one lump, data gets extended to a lot of slices and it can be extended to 64 MB.

## Compare MongoDB with Couchbase and CouchbaseDB.
Although MongoDB, Couchbase and Couchbase DB are common in many ways, still they are different in the case of necessities for the execution of the model, crossing points, storage, duplications, etc.

## When do we use a namespace in MongoDB?
During the sequencing of the names of the database and the collection, the namespace is used.

## If you remove an object attribute, is it deleted from the database?
Yes, it is deleted. Hence, it is better to eliminate the attribute and then save the object again.

## How can we move an old file into the moveChunk directory?
Once the functions are done, the old files are converted to backup files and moved to the moveChunk directory at the time of balancing the slices.

## Explain the situation when an index does not fit into RAM.
When an index is too huge to fit into RAM, then MongoDB reads the index, which is faster than reading RAM because the indexes easily fit into RAM if the server has got RAM for indexes, along with the remaining set.

## How does MongoDB provide consistency?
MongoDB uses the reader–writer locks, allowing simultaneous readers to access any supply like a database or a collection but always offering private access to single writes.

## Why is MongoDB not chosen for a 32-bit system?
Mongo DB is not considered as a 32-bit system because for running the 32-bit MongoDB, with the server, information and indexes require 2 GB. That is why it is not used in 32-bit devices.

## How does Journaling work in MongoDB?
Write operations are saved in memory while journaling is going on. The on-disk journal files are really dependable for the reason that the journal writes are habitual. Inside dbPath, a journal subdirectory is designed by MongoDB.

## How can you isolate the cursors from intervening with the write operations?
The snapshot() method is used to isolate the cursors from intervening with writes. This method negotiates the index and makes sure that each query comes to any article only once.

## what is CRUD?
MongoDB provides CRUD operations. CRUD is also a generic term in web apps.

* Create
* Read
* Update
* Delete



## Explain Replication.
Replication is the process of synchronizing data across multiple servers.

## What is the use of GridFS in MongoDB?
GridFS is used for storing and retrieving large files, such as audio, image, and video files.

## Which command is used for inserting a document in MongoDB?
The following command is used for inserting a document in MongoDB:

```
database.collection.insert (document)
```

## What type of data is stored by MongoDB?
MongoDB stores data in the form of documents, which are JSON-like field and value pairs.

## Define Horizontal Scaling.
Horizontal scaling divides the dataset and distributes data over multiple servers, or shards.

## Define the Aggregation pipeline.
The aggregation pipeline is a framework for performing aggregation tasks. The pipeline is used to transform documents into aggregated results.

## Define MapReduce.
MapReduce is a generic multi-phase data aggregation modality that is used for processing quantities of data.


## Pandas questions

### What are important data structures in pandas?

Pandas provide two data structures, which are supported by the pandas library, Series, and DataFrames. Both of these data structures are built on top of the NumPy.

A Series is a one-dimensional data structure in pandas, whereas the DataFrame is the two-dimensional data structure in pandas.

### what are Series in Pandas?
A Series is defined as a one-dimensional array that is capable of storing various data types. The row labels of series are called the index. By using a 'series' method, we can easily convert the list, tuple, and dictionary into series. A Series cannot contain multiple columns.

### What Is A pandas DataFrame? How Will You Create An Empty DataFrame In pandas?
pandas DataFrame is two-dimensional size-mutable, potentially heterogeneous tabular data structure with labeled axes (rows and columns). It consists of three principal components, the data, rows, and columns. pandas DataFrame can be created from the lists, dictionary, and from a list of dictionary, etc.

To create an empty DataFrame in pandas, type
```
import pandas as pd

df = pd.DataFrame()
```

### How do you Create a DataFrame using List?

We can create a DataFrame using following ways:

* Lists
* Dict of ndarrays

```
import pandas as pd    
# a list of strings    
a = ['Python', 'Pandas']    
# Calling DataFrame constructor on list    
info = pd.DataFrame(a)    
print(info)   
```

Using dict of ndarrays

```
import pandas as pd    
info = {'ID' :[101, 102, 103],'Department' :['B.Sc','B.Tech','M.Tech',]}    
info = pd.DataFrame(info)    
print (info)   
```

### How will you add a column to a pandas DataFrame?
We can add any new column to an existing DataFrame. The below code demonstrates how to add any new column to an existing DataFrame:

By importing the pandas library:

```
import pandas as pd      
info = {'one' : pd.Series([1, 2, 3, 4, 5], index=['a', 'b', 'c', 'd', 'e']),    
             'two' : pd.Series([1, 2, 3, 4, 5, 6], index=['a', 'b', 'c', 'd', 'e', 'f'])}    
   
info = pd.DataFrame(info)    
```


Add a new column to an existing DataFrame object     

```
print ("Add new column by passing series")    
info['three']=pd.Series([20,40,60],index=['a','b','c'])    
print (info)    
print ("Add new column using existing DataFrame columns")    
info['four']=info['one']+info['three']    
print (info)    
```

### How to Delete Indices, Rows or Columns From a Pandas Data Frame?
Deleting an Index from Your DataFrame

If you want to remove the index from the DataFrame, you should have to do the following:

Reset the index of DataFrame.

Executing del df.index.name to remove the index name.

Remove duplicate index values by resetting the index and drop the duplicate values from the index column.

Remove an index with a row.

Deleting a Column from Your DataFrame

You can use the drop() method for deleting a column from the DataFrame.

The axis argument that is passed to the drop() method is either 0 if it indicates the rows and 1 if it drops the columns.

You can pass the argument inplace and set it to True to delete the column without reassign the DataFrame.

You can also delete the duplicate values from the column by using the drop_duplicates() method.

Removing a Row from Your DataFrame

By using df.drop_duplicates(), we can remove duplicate rows from the DataFrame.

You can use the drop() method to specify the index of the rows that we want to remove from the DataFrame.

### How to get the items of series A not present in series B?
We can remove items present in p2 from p1 using isin() method.

### How to get the items not common to both series A and series B?
We get all the items of p1 and p2 not common to both using below example:

```
import pandas as pd  
import numpy as np  
p1 = pd.Series([2, 4, 6, 8, 10])  
p2 = pd.Series([8, 10, 12, 14, 16])  
p1[~p1.isin(p2)]  
p_u = pd.Series(np.union1d(p1, p2))  # union  
p_i = pd.Series(np.intersect1d(p1, p2))  # intersect  
p_u[~p_u.isin(p_i)]  
```

### How to get the minimum, 25th percentile, median, 75th, and max of a numeric series?
We can compute the minimum, 25th percentile, median, 75th, and maximum of p as below example:

```
import pandas as pd  
import numpy as np  
p = pd.Series(np.random.normal(14, 6, 22))  
state = np.random.RandomState(120)  
p = pd.Series(state.normal(14, 6, 22))  
np.percentile(p, q=[0, 25, 50, 75, 100])  
```


### How to convert a numpy array to a dataframe of given shape?
We can reshape the series p into a dataframe with 6 rows and 2 columns as below example:

```
import pandas as pd  
import numpy as np  
p = pd.Series(np.random.randint(1, 7, 35))  
# Input  
p = pd.Series(np.random.randint(1, 7, 35))  
info = pd.DataFrame(p.values.reshape(7,5))  
print(info)  

```


## Python related data engineering questions

### What Native Data Structures Can You Name in Python?
Common native data structures in Python are as follows:

```
Dictionaries
Lists
Sets
Strings
Tuples
```

### In a List and in a Dictionary, What Are the Typical Characteristics of Elements?
Elements in lists maintain their ordering unless they are explicitly commanded to be re-ordered. They can be of any data type, they can all be the same, or they can be mixed. Elements in lists are always accessed through numeric, zero-based indices.

In a dictionary, each entry will have a key and a value, but the order will not be guaranteed. Elements in the dictionary can be accessed by using their key.

Lists can be used whenever you have a collection of items in an order. A dictionary can be used whenever you have a set of unique keys that map to values.

### Is There a Way to Get a List of All the Keys in a Dictionary? If So, How Would You Do It?
If the interviewer follows up with this question, try to make your answer as specific as possible.

To obtain a list of all the keys in a dictionary, we have to use function keys():
```
mydict={‘a’:1,’b’:2,’c’:3,’e’:5}

mydict.keys()

dict_keys([‘a’, ‘b’, ‘c’, ‘e’])
```

### When Would You Use a List vs. a Tuple vs. a Set in Python?
A list is a common data type that is highly flexible. It can store a sequence of objects that are mutable, so it’s ideal for projects that demand the storage of objects that can be changed later.

A tuple is similar to a list in Python, but the key difference between them is that tuples are immutable. They also use less space than lists and can only be used as a key in a dictionary. Tuples are a perfect choice when you want a list of constants.

Sets are a collection of unique elements that are used in Python. Sets are a good option when you want to avoid duplicate elements in your list. This means that whenever you have two lists with common elements between them, you can leverage sets to eliminate them.

###  Compare BeautifulSoup and Scrapy

Scrapy is an open-source collaborative framework used to extract the data from a website. 
Scrapy is built on top of Twisted, which is an asynchronous networking framework. 
It has built-in support for extracting data from HTML sources using XPath expression and CSS expression.

BeautifulSoup is a library that makes it easy to scrape information from web pages. It sits atop an HTML or XML parser, 
providing Pythonic idioms for iterating, searching, and modifying the parse tree.
It can help the programmer to quickly extract the data from a certain web page.
It is used with Requests or Urlib2 to make the request to the server.
It  requires an External parser to parse the downloaded data: lxml’s XML parser, lxml’s HTML parser, HTML5lib, HTML.parser.


###  Name a few libraries in python used for Data analysis and scientific computations

Here is a list of Python libraries mainly used for Data Analysis:

```
NumPy
SciPy
Pandas
SciKit
Matplotlib
Seaborn
Bokeh
```

### Which library would you prefer for plotting in Python language: Seaborn or Matplotlib or Bokeh?

It depends on the visualization you’re trying to achieve. Each of these libraries is used for a specific purpose:

* Matplotlib: Used for basic plotting like bars, pies, lines, scatter plots, etc
* Seaborn: Is built on top of Matplotlib and Pandas to ease data plotting. It is used for statistical visualizations like creating heatmaps or showing the distribution of your data
* Bokeh: Used for interactive visualization. In case your data is too complex and you haven’t found any “message” in the data, then use Bokeh to create interactive visualizations that will allow your viewers to explore the data themselves


### How are NumPy and SciPy related?
* NumPy is part of SciPy.
* NumPy defines arrays along with some basic numerical functions like indexing, sorting, reshaping, etc.
* SciPy implements computations such as numerical integration, optimization and machine learning using NumPy’s functionality.

### How can you handle duplicate values in a dataset for a variable in Python?
Consider the following Python code:

```
bill_data=pd.read_csv("datasetsTelecom Data AnalysisBill.csv")
bill_data.shape
#Identify duplicates records in the data
Dupes = bill_data.duplicated()
sum(dupes)
#Removing Duplicates
bill_data_uniq = bill_data.drop_duplicates()

```

### Write a basic Machine Learning program to check the accuracy of a model,  by importing any dataset using any classifier?

```
#importing dataset
import sklearn
from sklearn import datasets
iris = datasets.load_iris()
X = iris.data
Y = iris.target
 
#splitting the dataset
from sklearn.cross_validation import train_test_split
X_train, Y_train, X_test, Y_test = train_test_split(X,Y, test_size = 0.5)
 
#Selecting Classifier
my_classifier = tree.DecisionTreeClassifier()
My_classifier.fit(X_train, Y_train)
predictions = my_classifier(X_test)
#check accuracy
From sklear.metrics import accuracy_score
print accuracy_score(y_test, predictions)
```




## Spark questions

### What does a Spark Engine do?
A Spark engine is responsible for scheduling, distributing, and monitoring the data application across the cluster.

### What is RDD.
RDD is the acronym for Resilient Distribution Datasets—a fault-tolerant collection of operational elements that run in parallel. The partitioned data in an RDD is *immutable and distributed*.

Decomposing the name RDD:

* Resilient, i.e. fault-tolerant with the help of RDD lineage graph(DAG) and so able to recompute missing or damaged partitions due to node failures.
* Distributed, since Data resides on multiple nodes.
* Dataset represents records of the data you work with. The user can load the data set externally which can be either JSON file, CSV file, text file or database via JDBC with no specific data structure.


There are primarily two types of RDDs:

* Parallelized collections: The existing RDDs running in parallel with one another
* Hadoop datasets: Those performing a function on each file record in HDFS or any other storage system

RDD is a dataset which is distributed, that is, it is divided into "partitions". Each of these partitions can be present in the memory or disk of different machines. If you want Spark to process the RDD, then Spark needs to launch one task per partition of the RDD. Its best that each task be sent to the machine have the partition that task is supposed to process. In that case, the task will be able to read the data of the partition from the local machine. Otherwise, the task would have to pull the partition data over the network from a different machine, which is less efficient. This scheduling of tasks (that is, allocation of tasks to machines) such that the tasks can read data "locally" is known as "locality aware scheduling".

RDD is representation of set of records, immutable collection of objects with distributed computing. Resilient Distributed Datasets (RDD) is large collection of data or RDD is an array of reference of partitioned objects. Each and every datasets in RDD is logically partitioned across many servers so that they can be computed on different nodes of cluster. RDDs are fault tolerant i.e. self-recovered/recomputed in case of failure. Dataset could be data loaded externally by the users which can be in the form of json file, csv file, text file or database via JDBC with no specific data structure.

RDD Transformation is Lazily Evaluated i.e. it is memorized or called when required or needed which saves lots of time and improves overall efficiency. RDD is a read only, partitioned collection of data. RDD can be created through deterministic operations or on stable storage or other RDDs. It can be generated by parallelizing an existing collection in your driver program or referencing a dataset in an external storage system. It is cacheable.

Some Unique features:

1. In-memory Computation

Spark RDDs have a provision of in-memory computation. It stores intermediate results in distributed memory(RAM) instead of stable storage(disk).

2. Lazy Evaluations

All transformations in Apache Spark are lazy, in that they do not compute their results right away. Instead, they just remember the transformations applied to some base data set.

Spark computes transformations when an action requires a result for the driver program. Follow this guide for the deep study of Spark Lazy Evaluation.

3. Fault Tolerance

Spark RDDs are fault tolerant as they track data lineage information to rebuild lost data automatically on failure. They rebuild lost data on failure using lineage, each RDD remembers how it was created from other datasets (by transformations like a map, join or groupBy) to recreate itself. Follow this guide for the deep study of RDD Fault Tolerance.

4. Immutability

Data is safe to share across processes. It can also be created or retrieved anytime which makes caching, sharing & replication easy. Thus, it is a way to reach consistency in computations.

5. Partitioning

Partitioning is the fundamental unit of parallelism in Spark RDD. Each partition is one logical division of data which is mutable. One can create a partition through some transformations on existing partitions.

6. Persistence

Users can state which RDDs they will reuse and choose a storage strategy for them (e.g., in-memory storage or on Disk).

7. Coarse-grained Operations

It applies to all elements in datasets through maps or filter or group by operation

8. Location-Stickiness

RDDs are capable of defining placement preference to compute partitions. Placement preference refers to information about the location of RDD. The DAGScheduler places the partitions in such a way that task is close to data as much as possible. Thus, speed up computation.

## Why is RDD immutable in Spark?
Immutability rules out a big set of potential problems due to updates from multiple threads at once. Immutable data is definitely safe to share across processes.

They're not just immutable but a deterministic function of their input. This plus immutability also means the RDD's parts can be recreated at any time. This makes caching, sharing and replication easy.

These are significant design wins, at the cost of having to copy data rather than mutate it in place. Generally, that's a decent tradeoff to make: gaining the fault tolerance and correctness with no developer effort is worth spending memory and CPU on, since the latter are cheap.

A corollary: immutable data can as easily live in memory as on disk. This makes it reasonable to easily move operations that hit disk to instead use data in memory, and again, adding memory is much easier than adding I/O bandwidth.

Of course, an RDD isn't really a collection of data, but just a recipe for making data from other data. It is not literally computed by materializing every RDD completely. That is, a lot of the "copy" can be optimized away too.

The idea of an RDD has no origin in MapReduce.

### What operations does an RDD support?
* Transformations are lazy operations on an RDD that create one or many new RDDs. For example Map, filter, reduceByKey etc creates new RDD. RDD create a new dataset from an existing one. That executes on demand. That means they compute lazily. Whenever we perform any transformation on RDD, it creates a new RDD each time.
* Actions return final result of RDD computations. It triggers execution using lineage graph to load the data into original RDD. After application of all the intermediate transformation, it gives the final result to driver program or writes it out to file system. Upon applying Actions on an RDD non-RDD values gets generate.

### What is the difference in cache() and persist() methods in Apache Spark?

Caching or Persistence are optimization techniques for (iterative and interactive) Spark computations. They help saving interim partial results so they can be reused in subsequent stages. These interim results as RDDs are thus kept in memory (default) or more solid storage like disk and/or replicated.

RDDs can be cached using cache operation. They can also be persisted using persist operation.

The difference between cache and persist operations is purely syntactic. cache is a synonym of persist or persist(MEMORY_ONLY), i.e. cache is merely persist with the default storage level MEMORY_ONLY while Persist provide you various following options:

* MEMORY_ONLY(Default level)
This option stores RDD in available cluster memory as deserialized Java objects. Some partitions may not be cached if there is not enough cluster memory. Those partitions will be recalculated on the fly as needed.

* MEMORY_AND_DISK
This option stores RDD as deserialized Java objects. If RDD does not fit in cluster memory, then store those partitions on the disk and read them as needed.

* MEMORY_ONLY_SER
This options stores RDD as serialized Java objects (One byte array per partition). This is more CPU intensive but saves memory as it is more space efficient. Some partitions may not be cached. Those will be recalculated on the fly as needed.

* MEMORY_ONLY_DISK_SER
This option is same as above except that disk is used when memory is not sufficient.

* DISC_ONLY
This option stores the RDD only on the disk.

* MEMORY_ONLY_2, MEMORY_AND_DISK_2
Same as other levels but partitions are replicated on 2 slave nodes.

### What the functions of Spark Core.
Serving as the base engine, Spark Core performs various important functions like memory management, monitoring jobs, providing fault-tolerance, job scheduling, and interaction with storage systems.

### Does spark support data replication in memory?

No


### What is RDD Lineage?
Spark does not support data replication in memory and thus, if any data is lost, it is *rebuilt* using RDD lineage. RDD lineage is a process that reconstructs lost data partitions. The best thing about this is that RDDs always remember how to build from other datasets.

### What is Spark Driver?
Spark driver is the program that runs on the master node of a machine and declares transformations and actions on data RDDs. In simple terms, a driver in Spark creates SparkContext, connected to a given Spark Master. It also delivers RDD graphs to Master, where the standalone Cluster Manager runs.

### What is Hive on Spark?
Hive contains significant support for Apache Spark, wherein Hive execution is configured to Spark:
```
hive> set spark.home=/location/to/sparkHome;
hive> set hive.execution.engine=spark;
Hive supports Spark on YARN mode by default.
```

### Name the commonly used Spark Ecosystems.
* Spark SQL (Shark) for developers
* Spark Streaming for processing live data streams
* GraphX for generating and computing graphs
* MLlib (Machine Learning Algorithms)
* SparkR to promote R programming in the Spark engine

### What is Spark Streaming.
Spark supports stream processing—an extension to the Spark API allowing stream processing of live data streams. Data from different sources like Kafka, Flume, Kinesis is processed and then pushed to file systems, live dashboards, and databases. It is similar to batch processing in terms of the input data which is here divided into streams like batches in batch processing.

### What is a Parquet file?
Parquet is a columnar format file supported by many other data processing systems. Spark SQL performs both read and write operations with the Parquet file and considers it be one of the best Big Data Analytics formats so far.

### What file systems does Apache Spark support?
* Hadoop Distributed File System (HDFS)
* Local file system
* Amazon S3

### What is YARN?
Similar to Hadoop, YARN is one of the key features in Spark, providing a central and resource management platform to deliver scalable operations across the cluster. Running Spark on YARN needs a binary distribution of Spark that is built on YARN support.

### List the functions of Spark SQL.
Spark SQL is capable of:

* Loading data from a variety of structured sources
* Querying data using SQL statements, both inside a Spark program and from external tools that connect to Spark SQL through standard database connectors (JDBC/ODBC), e.g., using Business Intelligence tools like Tableau
* Providing rich integration between SQL and the regular Python/Java/Scala code, including the ability to join RDDs and SQL tables, expose custom functions in SQL, and more.

Spark SQL doesn't do everything -- for instance, while Spark has SQL, engines such as Impala or HAWQ are still more efficient for random access, and interactive query.

### What are the benefits of Spark over MapReduce?
Due to the availability of in-memory processing, Spark implements data processing 10–100x faster than Hadoop MapReduce. MapReduce, on the other hand, makes use of persistence storage for any of the data processing tasks.
Unlike Hadoop, Spark provides in-built libraries to perform multiple tasks using batch processing, steaming, Machine Learning, and interactive SQL queries. However, Hadoop only supports batch processing.
Hadoop is highly disk-dependent, whereas Spark promotes caching and in-memory data storage.
Spark is capable of performing computations multiple times on the same dataset, which is called iterative computation. Whereas, there is no iterative computing implemented by Hadoop.

### Is there any benefit of learning MapReduce?
Yes, MapReduce is a paradigm used by many Big Data tools, including Apache Spark. It becomes extremely relevant to use MapReduce when data grows bigger and bigger. Most tools like Pig and Hive convert their queries into MapReduce phases to optimize them better.

### What is Spark Executor?
When SparkContext connects to Cluster Manager, it acquires an executor on the nodes in the cluster. Executors are Spark processes that run computations and store data on worker nodes. The final tasks by SparkContext are transferred to executors for their execution.

### Name the types of Cluster Managers in Spark.
The Spark framework supports three major types of Cluster Managers.

* Standalone: A basic Cluster Manager to set up a cluster
* Apache Mesos: A generalized/commonly-used Cluster Manager, running Hadoop MapReduce and other applications
* YARN: A Cluster Manager responsible for resource management in Hadoop

###  What is PageRank?
A unique feature and algorithm in GraphX, PageRank is the measure of each vertex in a graph. For instance, an edge from u to v represents an endorsement of v‘s importance w.r.t. u. In simple terms, if a user at Instagram is followed massively, he/she will be ranked high on that platform.

### Do you need to install Spark on all the nodes of the YARN cluster while running Spark on YARN?
No, because Spark runs on top of YARN.

### Illustrate some demerits of using Spark.
Since Spark utilizes more storage space when compared to Hadoop and MapReduce, there might arise certain problems. Developers need to be careful while running their applications on Spark. To resolve the issue, they can think of distributing the workload over multiple clusters, instead of running everything on a single node.

### How to create an RDD?
Spark provides two methods to create an RDD:

* By parallelizing a collection in the driver program. This makes use of SparkContext’s ‘parallelize’ method
```
val IntellipaatData = Array(2,4,6,8,10)
val distIntellipaatData = sc.parallelize(IntellipaatData)
```

By loading an external dataset from external storage like HDFS, the shared file system

### additional questions

https://www.edureka.co/blog/interview-questions/top-apache-spark-interview-questions-2016/

https://acadgild.com/blog/top-20-apache-spark-interview-questions-2019

https://mindmajix.com/apache-spark-interview-questions

https://www.toptal.com/spark/interview-questions

https://data-flair.training/blogs/apache-spark-interview-questions-and-answers/


## SQL questions

### what are different kinds of statements in SQL?

1. DDL, data definition language.  Used to characterize the database structure, tables.  Create, Alter and Drop.
2. DML, data manipulation language. Used to control the data in tables. Insert, Update, and Delete.
3. DCL, data control language. Used to set beenfits. Grant and Revoke database.

### What is a Primary Key? Can there be more than one Primary key?

The PRIMARY KEY constraint uniquely identifies each row in a table. It must contain UNIQUE values and has an implicit NOT NULL constraint.
A table in SQL is strictly restricted to have one and only one primary key, which is comprised of single or multiple fields (columns).

### What is a Foreign Key?

A FOREIGN KEY comprises of single or collection of fields in a table that essentially refer to the PRIMARY KEY in another table. Foreign key constraint ensures referential integrity in the relation between two tables.
The table with the foreign key constraint is labelled as the child table, and the table containing the candidate key is labelled as the referenced or parent table.

### What is a Join? List its different types.

The SQL Join clause is used to combine records (rows) from two or more tables in a SQL database based on a related column between the two.

There are four different types of JOINs in SQL:

* (INNER) JOIN: Retrieves records that have matching values in both tables involved in the join. This is the widely used join for queries.

```sql
SELECT *
FROM Table_A
JOIN Table_B;

SELECT *
FROM Table_A
INNER JOIN Table_B;
```

* LEFT (OUTER) JOIN: Retrieves all the records/rows from the left and the matched records/rows from the right table.

```sql
SELECT *
FROM Table_A A
LEFT JOIN Table_B B
ON A.col = B.col;
```

* RIGHT (OUTER) JOIN: Retrieves all the records/rows from the right and the matched records/rows from the left table.

```sql
SELECT *
FROM Table_A A
RIGHT JOIN Table_B B
ON A.col = B.col;
```

* FULL (OUTER) JOIN: Retrieves all the records where there is a match in either the left or right table.

```sql
SELECT *
FROM Table_A A
FULL JOIN Table_B B
ON A.col = B.col;
```

### What is a Self-Join?

A self JOIN is a case of regular join where a table is joined to itself based on some relation between its own column(s). Self-join uses the INNER JOIN or LEFT JOIN clause and a table alias is used to assign different names to the table within the query.

```sql
SELECT A.emp_id AS "Emp_ID",A.emp_name AS "Employee",
B.emp_id AS "Sup_ID",B.emp_name AS "Supervisor"
FROM employee A, employee B
WHERE A.emp_sup = B.emp_id;
```


### What is a Cross-Join?

Cross join can be defined as a cartesian product of the two tables included in the join. The table after join contains the same number of rows as in the cross-product of number of rows in the two tables. If a WHERE clause is used in cross join then the query will work like an INNER JOIN.

```sql
SELECT stu.name, sub.subject 
FROM students AS stu
CROSS JOIN subjects AS sub;
```




### What is the difference between Clustered and Non-clustered index?

Unique and Non-Unique Index:
Unique indexes are indexes that help maintain data integrity by ensuring that no two rows of data in a table have identical key values. Once a unique index has been defined for a table, uniqueness is enforced whenever keys are added or changed within the index.

Clustered and Non-Clustered Index:
Clustered indexes are indexes whose order of the rows in the database correspond to the order of the rows in the index. This is why only one clustered index can exist in a given table, whereas, multiple non-clustered indexes can exist in the table.

The only difference between clustered and non-clustered indexes is that the database manager attempts to keep the data in the database in the same order as the corresponding keys appear in the clustered index.

Clustering index can improve the performance of most query operations because they provide a linear-access path to data stored in the database.

Clustered index modifies the way records are stored in a database based on the indexed column. Non-clustered index creates a separate entity within the table which references the original table.

Clustered index is used for easy and speedy retrieval of data from the database, whereas, fetching records from the non-clustered index is relatively slower.
In SQL, a table can have a single clustered index whereas it can have multiple non-clustered indexes.

### What are some common clauses used with SELECT query in SQL?
Some common SQL clauses used in conjuction with a SELECT query are as follows:

```
WHERE clause in SQL is used to filter records that are necessary, based on specific conditions.
ORDER BY clause in SQL is used to sort the records based on some field(s) in ascending (ASC) or descending order (DESC).
SELECT *
FROM myDB.students
WHERE graduation_year = 2019
ORDER BY studentID DESC;
```

GROUP BY clause in SQL is used to group records with identical data and can be used in conjuction with some aggregation functions to produce summarized results from the database.
HAVING clause in SQL is used to filter records in combination with the GROUP BY clause. It is different from WHERE, since WHERE clause cannot filter aggregated records.

```
SELECT COUNT(studentId), country
FROM myDB.students
WHERE country != "INDIA"
GROUP BY country
HAVING COUNT(studentID) > 5;
```
### What are UNION, MINUS and INTERSECT commands?
The UNION operator combines and returns the result-set retrieved by two or more SELECT statements.
The MINUS operator in SQL is used to remove duplicates from the result-set obtained by the second SELECT query from the result-set obtained by the first SELECT query and then return the filtered results from the first.
The INTERSECT clause in SQL combines the result-set fetched by the two SELECT statements where records from one match the other and then returns this intersection of result-sets.

Certain conditions need to be met before executing either of the above statements in SQL -

Each SELECT statement within the clause must have the same number of columns
The columns must also have similar data types
The columns in each SELECT statement should necessarily have the same order
```
SELECT name FROM Students 	 /* Fetch the union of queries */
UNION
SELECT name FROM Contacts;
```

```
SELECT name FROM Students 	 /* Fetch the union of queries with duplicates*/
UNION ALL
SELECT name FROM Contacts;
```

```
SELECT name FROM Students 	 /* Fetch names from students */
MINUS 				/* that aren't present in contacts */
SELECT name FROM Contacts;
```

```
SELECT name FROM Students 	 /* Fetch names from students */
INTERSECT 			/* that are present in contacts as well */
SELECT name FROM Contacts;
```

### What is Cursor? How to use a Cursor?
A database cursor is a control structure that allows for traversal of records in a database. Cursors, in addition, facilitates processing after traversal, such as retrieval, addition and deletion of database records. They can be viewed as a pointer to one row in a set of rows.

Working with SQL Cursor:

* DECLARE a cursor after any variable declaration. The cursor declaration must always be associated with a SELECT Statement.
* Open cursor to initialize the result set. The OPEN statement must be called before fetching rows from the result set.
* FETCH statement to retrieve and move to the next row in the result set.
* Call the CLOSE statement to deactivate the cursor.
* Finally use the DEALLOCATE statement to delete the cursor definition and release the associated resources.


```
DECLARE @name VARCHAR(50) 	 /* Declare All Required Variables */

DECLARE db_cursor CURSOR FOR 	 /* Declare Cursor Name*/
SELECT name
FROM myDB.students
WHERE parent_name IN ('Sara', 'Ansh')

OPEN db_cursor 	 /* Open cursor and Fetch data into @name */ 
FETCH next
FROM db_cursor
INTO @name

CLOSE db_cursor 	 /* Close the cursor and deallocate the resources */
DEALLOCATE db_cursor
```

### What are Entities and Relationships?
Entity: An entity can be a real-world object, either tangible or intangible, that can be easily identifiable. For example, in a college database, students, professors, workers, departments, and projects can be referred to as entities. Each entity has some associated properties that provide it an identity.

Relationships: Relations or links between entities that have something to do with each other. For example - The employees table in a company's database can be associated with the salary table in the same database.

### List the different types of relationships in SQL.
* One-to-One - This can be defined as the relationship between two tables where each record in one table is associated with the maximum of one record in the other table.
* One-to-Many & Many-to-One - This is the most commonly used relationship where a record in a table is associated with multiple records in the other table.
* Many-to-Many - This is used in cases when multiple instances on both sides are needed for defining a relationship.
Self Referencing Relationships - This is used when a table needs to define a relationship with itself.

### What is a View?
A view in SQL is a virtual table based on the result-set of an SQL statement. A view contains rows and columns, just like a real table. The fields in a view are fields from one or more real tables in the database.

### What is Normalization?
Normalization represents the way of organizing structured data in the database efficiently. It includes creation of tables, establishing relationships between them, and defining rules for those relationships. Inconsistency and redundancy can be kept in check based on these rules, hence, adding flexibility to the database.

### What is Denormalization?
Denormalization is the inverse process of normalization, where the normalized schema is converted into a schema which has redundant information. The performance is improved by using redundancy and keeping the redundant data consistent. The reason for performing denormalization is the overheads produced in query processor by an over-normalized structure.

### What are the TRUNCATE, DELETE and DROP statements?
DELETE statement is used to delete rows from a table.

```
DELETE FROM Candidates
WHERE CandidateId > 1000;
```


TRUNCATE command is used to delete all the rows from the table and free the space containing the table.

```
TRUNCATE TABLE Candidates;
```


DROP command is used to remove an object from the database. If you drop a table, all the rows in the table is deleted and the table structure is removed from the database.


```
DROP TABLE Candidates;
```


### What is the difference between DROP and TRUNCATE statements?
If a table is dropped, all things associated with the tables are dropped as well. This includes - the relationships defined on the table with other tables, the integrity checks and constraints, access privileges and other grants that the table has. To create and use the table again in its original form, all these relations, checks, constraints, privileges and relationships need to be redefined. However, if a table is truncated, none of the above problems exist and the table retains its original structure.

### What is the difference between DELETE and TRUNCATE statements?
The TRUNCATE command is used to delete all the rows from the table and free the space containing the table.
The DELETE command deletes only the rows from the table based on the condition given in the where clause or deletes all the rows from the table if no condition is specified. But it does not free the space containing the table.

### What are Aggregate and Scalar functions?
An aggregate function performs operations on a collection of values to return a single scalar value. Aggregate functions are often used with the GROUP BY and HAVING clauses of the SELECT statement. Following are the widely used SQL aggregate functions:

```
AVG() - Calculates the mean of a collection of values.
COUNT() - Counts the total number of records in a specific table or view.
MIN() - Calculates the minimum of a collection of values.
MAX() - Calculates the maximum of a collection of values.
SUM() - Calculates the sum of a collection of values.
FIRST() - Fetches the first element in a collection of values.
LAST() - Fetches the last element in a collection of values.
Note: All aggregate functions described above ignore NULL values except for the COUNT function.
```

A scalar function returns a single value based on the input value. Following are the widely used SQL scalar functions:

```
LEN() - Calculates the total length of the given field (column).
UCASE() - Converts a collection of string values to uppercase characters.
LCASE() - Converts a collection of string values to lowercase characters.
MID() - Extracts substrings from a collection of string values in a table.
CONCAT() - Concatenates two or more strings.
RAND() - Generates a random collection of numbers of given length.
ROUND() - Calculates the round off integer value for a numeric field (or decimal point values).
NOW() - Returns the current data & time.
FORMAT() - Sets the format to display a collection of values.

```

### What are transactions and its controls?

Transaction is the grouping assignment that is performed on databases.  The controls are: COMMIT,
ROLLBACK, SET TRANSACTION, SAVEPOINT.

### What are 4 kinds of relations.

* One to many
* Many to One
* Many to Many
* One to One

### What is User-defined function? What are its various types?
Scalar Function: As explained earlier, user-defined scalar functions return a single scalar value.
Table Valued Functions: User-defined table-valued functions return a table as output.
Inline: returns a table data type based on a single SELECT statement.
Multi-statement: returns a tabular result-set but, unlike inline, multiple SELECT statements can be used inside the function body.


### What is OLTP?
OLTP stands for Online Transaction Processing, is a class of software applications capable of supporting transaction-oriented programs. An essential attribute of an OLTP system is its ability to maintain concurrency. To avoid single points of failure, OLTP systems are often decentralized. These systems are usually designed for a large number of users who conduct short transactions. Database queries are usually simple, require sub-second response times and return relatively few records. 

### What are the differences between OLTP and OLAP?
OLTP stands for Online Transaction Processing, is a class of software applications capable of supporting transaction-oriented programs. An important attribute of an OLTP system is its ability to maintain concurrency. OLTP systems often follow a decentralized architecture to avoid single points of failure. These systems are generally designed for a large audience of end users who conduct short transactions. Queries involved in such databases are generally simple, need fast response times and return relatively few records. Number of transactions per second acts as an effective measure for such systems.

OLAP stands for Online Analytical Processing, a class of software programs which are characterized by relatively low frequency of online transactions. Queries are often too complex and involve a bunch of aggregations. For OLAP systems, the effectiveness measure relies highly on response time. Such systems are widely used for data mining or maintaining aggregated, historical data, usually in multi-dimensional schemas.

### What is Collation? What are the different types of Collation Sensitivity?
Collation refers to a set of rules that determine how data is sorted and compared. Rules defining the correct character sequence are used to sort the character data. It incorporates options for specifying case-sensitivity, accent marks, kana character types and character width. Below are the different types of collation sensitivity:

```
Case sensitivity: A and a are treated differently.
Accent sensitivity: a and á are treated differently.
Kana sensitivity: Japanese kana characters Hiragana and Katakana are treated differently.
Width sensitivity: Same character represented in single-byte (half-width) and double-byte (full-width) are treated differently.
```

### What is a Stored Procedure?
A stored procedure is a subroutine available to applications that access a relational database management system (RDBMS). Such procedures are stored in the database data dictionary. The sole disadvantage of stored procedure is that it can be executed nowhere except in the database and occupies more memory in the database server. It also provides a sense of security and functionality as users who can't access the data directly can be granted access via stored procedures.

```
DELIMITER $$
CREATE PROCEDURE FetchAllStudents()
BEGIN
SELECT *  FROM myDB.students;
END $$
DELIMITER ;
```


### What is Pattern Matching in SQL?
SQL pattern matching provides for pattern search in data if you have no clue as to what that word should be. This kind of SQL query uses wildcards to match a string pattern, rather than writing the exact word. The LIKE operator is used in conjunction with SQL Wildcards to fetch the required information.

* Using the % wildcard to perform a simple search

The % wildcard matches zero or more characters of any type and can be used to define wildcards both before and after the pattern. Search a student in your database with first name beginning with the letter K:

```
SELECT *
FROM students
WHERE first_name LIKE 'K%'

```

* Omitting the patterns using the NOT keyword

Use the NOT keyword to select records that don't match the pattern. This query returns all students whose first name does not begin with K.

```
SELECT *
FROM students
WHERE first_name NOT LIKE 'K%'
```

* Matching a pattern anywhere using the % wildcard twice

Search for a student in the database where he/she has a K in his/her first name.

```
SELECT *
FROM students
WHERE first_name LIKE '%Q%'
```


*Using the _ wildcard to match pattern at a specific position

The _ wildcard matches exactly one character of any type. It can be used in conjunction with % wildcard. This query fetches all students with letter K at the third position in their first name.

```
SELECT *
FROM students
WHERE first_name LIKE '__K%'
```


* Matching patterns for specific length

The _ wildcard plays an important role as a limitation when it matches exactly one character. It limits the length and position of the matched results. For example -


```
SELECT * 	 /* Matches first names with three or more letters */
FROM students
WHERE first_name LIKE '___%'

SELECT * 	 /* Matches first names with exactly four characters */
FROM students
WHERE first_name LIKE '____'

```

### Write an SQL query that makes recommendations using the pages that your friends liked. Assume you have two tables: a two-column table of users and their friends, and a two-column table of users and the pages they liked. It should not recommend pages you already like.

```
SELECT f.user_id, l.page_id
FROM friend f JOIN like l
ON f.friend_id = l.user_id
WHERE l.page_id NOT IN (SELECT page_id FROM like
WHERE user_id = f.user_id)
```



### Find the month-over-month percentage change for monthly active users (MAU). 

Context: Oftentimes it's useful to know how much a key metric, such as monthly active users, changes between months. Say we have a table logins in the form: 

| user_id | date       |
|---------|------------|
| 1       | 2018-07-01 |
| 234     | 2018-07-02 |
| 3       | 2018-07-02 |
| 1       | 2018-07-02 |
| ...     | ...        |
| 234     | 2018-10-04 |

Solution:

```
WITH mau AS 
(
  SELECT 
   /* 
    * Typically, interviewers allow you to write psuedocode for date functions 
    * i.e. will NOT be checking if you have memorized date functions. 
    * Just explain what your function does as you whiteboard 
    *
    * DATE_TRUNC() is available in Postgres, but other SQL date functions or 
    * combinations of date functions can give you a identical results   
    * See https://www.postgresql.org/docs/9.0/functions-datetime.html#FUNCTIONS-DATETIME-TRUNC
    */ 
    DATE_TRUNC('month', date) month_timestamp,
    COUNT(DISTINCT user_id) mau
  FROM 
    logins 
  GROUP BY 
    DATE_TRUNC('month', date)
  )
 
 SELECT 
    /*
    * You don't literally need to include the previous month in this SELECT statement. 
    * 
    * However, as mentioned in the "Tips" section of this guide, it can be helpful 
    * to at least sketch out self-joins to avoid getting confused which table 
    * represents the prior month vs current month, etc. 
    */ 
    a.month_timestamp previous_month, 
    a.mau previous_mau, 
    b.month_timestamp current_month, 
    b.mau current_mau, 
    ROUND(100.0*(b.mau - a.mau)/a.mau,2) AS percent_change 
 FROM
    mau a 
 JOIN 
    /*
    * Could also have done `ON b.month_timestamp = a.month_timestamp + interval '1 month'` 
    */
    mau b ON a.month_timestamp = b.month_timestamp - interval '1 month' 
```


### Write SQL such that each node can be left, inner, or Root node, for input table that has node number and parent node id.

Context: you have a table "tree" with a column of nodes and a column corresponding parent nodes

node  | parent
--- | ---
1   |    2
2   |    5
3    |   5
4    |   3
5   |    NULL 

 Write SQL such that we label each node as a “leaf”, “inner” or “Root” node, such that for the nodes above we get: 

node |   label  
---|---
1   |    Leaf
2   |    Inner
3   |    Inner
4   |    Leaf
5   |    Root

A solution which works for the above example will receive full credit, although you can receive extra credit for providing a solution that is generalizable to a tree of any depth (not just depth = 2, as is the case in the example above). 

Solution: This solution works for the example above with tree depth = 2, but is not generalizable beyond that. 

```
WITH join_table AS 
(
SELECT 
    a.node a_node,
    a.parent a_parent,
    b.node b_node, 
    b.parent b_parent
 FROM
    tree a 
 LEFT JOIN 
    tree b ON a.parent = b.node 
 )
 
 SELECT 
    a_node node, 
    CASE 
        WHEN b_node IS NULL and b_parent IS NULL THEN 'Root'
        WHEN b_node IS NOT NULL and b_parent IS NOT NULL THEN 'Leaf'        
        ELSE 'Inner' 
    END AS label 
 FROM 
    join_table 
        
```


Alternate solution: more general

```
WITH join_table AS
(
    SELECT 
        cur.node, 
        cur.parent, 
        COUNT(next.node) AS num_children
    FROM 
        tree cur
    LEFT JOIN 
        tree next ON (next.parent = cur.node)
    GROUP BY 
        cur.node, 
        cur.parent
)

SELECT
    node,
    CASE
        WHEN parent IS NULL THEN "Root"
        WHEN num_children = 0 THEN "Leaf"
        ELSE "Inner"
    END AS label
FROM 
    join_table 
```

Alternate alternate:

```
SELECT 
    node,
    CASE 
        WHEN parent IS NULL THEN 'Root'
        WHEN node NOT IN 
            (SELECT parent FROM tree WHERE parent IS NOT NULL) THEN 'Leaf'
        WHEN node IN (SELECT parent FROM tree) AND parent IS NOT NULL THEN 'Inner'
    END AS label 
 from 
    tree
```

More of these types of questions at 
https://quip.com/2gwZArKuWk7W

At https://www.interviewbit.com/sql-interview-questions/

# data engineering verbal questions

## General questions and strategy

Study the resume of the candidate and initially ask questions to learn about the level of the candidate to 
figure out what kind of questions can be fairly asked of the candidate. We want the candidate to be
able to help us in our practice. We want candidates that will contribute well to the team. But we
also don't want to ask questions that candidate is obviously not going to be able to answer. We can ask
any question here. But be prepared to adjust the level of questions. We want effective question and answers
that are relevant in the sense of learning how the candidate can contribute and help us. 

For example, if the candidate is clearly not able to talk about SQL or Hadoop in any way, having had no
such background, then it is not good to insist on asking detailed SQL or Hadoop questions.

If the resume suggests data engineering background not yet covered in the following list of questions,
please prepare some new questions and add to the list below.   For example, a candidate might have no SQL
or Hadoop experience but have some python and numpy experience.  We can add some pandas and numpy questions.
They are relevant to the candidate's experience.

In the worst case, we can ask very generic questions that are general data engineering related questions. These
should be listed towards the top of the question list below.

### What is data engineering?

Data engineering is a software engineering approach to developing and designing information systems. It focuses on the collection and analysis of data. While data scientists perform various tasks with big data, someone has to collect all of this data before, and data engineers perform that task. Data engineers are responsible for the development and maintenance of databases as well. Data engineers convert raw data into usable data. 


### What are the most important languages/skills you’ve learned and use on a daily basis?
Data engineers use a variety of languages and skills. Use this interview question to learn which languages they are most skilled/comfortable with using. 

### Describe some of the projects from your current role. How do you think you’ll be able to apply your experience there with our company?
This data engineer interview question lets your candidate tell you in their own words why they’re a fit for your open position. Make sure to gain insight into their previous work experience and how it applies to your role.

### What are some of the most common problems you’ve run into with your work? What’s the biggest problem you’ve ever run into? How did you overcome these challenges?
Learning about challenges and how your candidate has overcome them can speak towards their creativity, resilience, and fit for your company. This data engineer interview question showcases their competency in data engineering and problem solving skills. 

### Can you describe a time where you found a new use case for an existing database?
This interview question shows you how a candidate has helped create positive impacts at their previous companies using existing databases.  

### What Is the Biggest Challenge Facing Your Current Job Right Now? What Is Your Biggest Failure?
This question comes up often regardless of the field because it helps the interviewer get an idea of your approach to problem-solving in your new potential role. The way you approach the answer will make you look awesome, or it will be a red flag. So it will be critical to think about this beforehand and answer the question without delay.

As a rule, don’t complain about the management at your current job or blame the people you’re working with. It’s also not a good idea to pretend like your career has been a walk in the park. Instead, tailor your answer to a project you worked on, but don’t get specific about why the challenge turned out to be difficult in the first place. Instead, concentrate on the problem-solving process to highlight your skills.

When it comes to your biggest failure, it’s critical that you don’t use this time to talk yourself down. If you can’t think of a specific scenario, think of a time when you were disappointed about something that didn’t work out. The primary objective is to show the interviewer how you managed to turn something negative into something positive.

### What Is the Accomplishment You Are Most Proud Of?
This interview question is designed to test your storytelling skills in the context of a professional example. So it’s important to start by setting the stage for your example. You can do this by talking about where you were working at the time, the project you were working on, the people you worked with, how you worked (tools, processes, the time taken), and the specific results.

You will have to think on your feet as there may well be follow-up questions, so be prepared to dive in and get into the nitty-gritty details. It’s essential to use a recent example here, so keep it fresh and give the recruiter a chance to imagine your future success based on your past work experience.

### What are some of your favorite programming languages and frameworks? Do you have a github or gitlab URL?

Do you have a git repository you are interested in sharing that show your best work?

Why do you like the language X over Y?  Framework A over B?

What is Pull request or Merge request and how do they work in a distributed software development in the context of a team that uses git?

What is git bisect, git stash, git rebase, git cherry pick?

What is difference between gitflow and github flow?  gitflow and gitlab flow?  Why the differences?


### What is CAP theorem in the context of distributed databases ?


CAP stands for:
* Consistency refers to whether a system operates fully or not. Does the system reliably follow the established rules within its programming according to those defined rules?  Do all nodes within a cluster see all the data they are supposed to? This is the same idea presented in ACID.
* Availability means just as it sounds. Is the given service or system available when requested? Does each request get a response outside of failure or success?
* Partition Tolerance represents the fact that a given system continues to operate even under circumstances of data loss or system failure. A single node failure should not cause the entire system to collapse.

Make the point that in the majority of instances, a distributed system can only guarantee two of the features, not all three. 

CA: RDBMS
AP: CouchDB, Cassandra, DynamoDB, Riak
CP: MongoDB, HBase, Redis

### Why can a system not have all three properties of the CAP theorem?



### What is ACID in the context of databases?

ACID stands for:

* Atomicity: Either the task (or all tasks) within a transaction are performed or none of them are. This is the all-or-none principle. If one element of a transaction fails the entire transaction fails.
* Consistency: The transaction must meet all protocols or rules defined by the system at all times. The transaction does not violate those protocols and the database must remain in a consistent state at the beginning and end of a transaction; there are never any half-completed transactions.
* Isolation: No transaction has access to any other transaction that is in an intermediate or unfinished state. Thus, each transaction is independent unto itself. This is required for both performance and consistency of transactions within a database.
* Durability: Once the transaction is complete, it will persist as complete and cannot be undone; it will survive system failure, power loss and other types of system breakdowns.

### what does BASE mean in database as opposed to ACID in the context of databases?



BASE stands for:
* Basically Available: This constraint states that the system does guarantee the availability of the data as regards CAP Theorem; there will be a response to any request. But, that response could still be ‘failure’ to obtain the requested data or the data may be in an inconsistent or changing state, much like waiting for a check to clear in your bank account.
* Soft state: The state of the system could change over time, so even during times without input there may be changes going on due to ‘eventual consistency,’ thus the state of the system is always ‘soft.’
* Eventual consistency: The system will eventually become consistent once it stops receiving input. The data will propagate to everywhere it should sooner or later, but the system will continue to receive input and is not checking the consistency of every transaction before it moves onto the next one. Werner Vogel’s article “Eventually Consistent – Revisited” covers this topic is much greater detail.


### what is Cloud SQL?
Cloud SQL is a fully managed database service that makes it easy to set up and manage your relational PostgreSQL, MySQL, and SQL Server databases in the cloud.

Ideal for
WordPress, backends, game states, CRM tools, MySQL, PostgreSQL, and Microsoft SQL Servers

Compare to
AWS RDS, AWS Aurora, Azure Database, Azure SQL Database

### what is Cloud Bigtable?
Cloud Bigtable is a NoSQL database service for use cases where low latency reads and high throughput writes, scalability, and reliability are critical.

Ideal for
running large analytical workloads and building low-latency applications


Compare  to
HBase, Cassandra, AWS DynamoDB, Azure CosmosDB


### what is Cloud Spanner?
Cloud Spanner is a scalable relational database service built to support transactions, strong consistency, and high availability across regions and continents.

Ideal for
teams requiring scale insurance and mission-critical availability

Compare to
Cassandra (with CQL), AWS Aurora, AWS DynamoDB, Azure CosmosDB


### what is Cloud Memorystore?
Cloud Memorystore is a fully managed in-memory data store service for Redis built on scalable, more secure, and highly available infrastructure.

Ideal for
building application caches and sub-millisecond data access using Redis
Compare to
AWS Elasticache, Azure Cache


### what is Cloud Firestore?
Cloud Firestore is a fast, fully managed, serverless, cloud-native NoSQL document database.

Ideal for
building client side mobile and web applications, gaming leaderboards, and user presence at global scale
Compare to
MongoDB, AWS DynamoDB, Azure CosmosDB


### what is Firebase Realtime Database?
The Firebase Realtime Database is a cloud-hosted NoSQL database that lets you store and sync data between your users in real time.

Ideal for
creating onboarding flows, rolling out new features, and building serverless apps
Compare to
MongoDB, AWS DynamoDB, Azure Cosmos DB

### what is BigQuery?
BigQuery is a serverless, highly scalable, and cost-effective data warehouse designed to help you make informed decisions quickly.

Ideal for
real-time analytics, advanced and predictive analytics, large-scale events, and enterprises
Compare to
AWS Redshift, Snowflake, and Azure SQL Data Warehouse














# Cloud

https://www.javatpoint.com/cloud-computing-interview-questions

## general cloud related questions

https://www.acte.in/google-cloud-interview-questions-and-answers

https://www.javatpoint.com/cloud-computing-interview-questions

https://www.javatpoint.com/cloud-service-models


# Frontend

https://frontendmasters.com/books/front-end-handbook/2018/practice/interview-q.html
# Backend

https://www.fullstack.cafe/blog/backend-developer-interview-questions

# Networking

https://www.indeed.com/career-advice/interviewing/hardware-and-networking-interview-questions

https://www.softwaretestinghelp.com/networking-interview-questions-2/

https://www.naukri.com/learning/articles/networking-interview-questions-answers/


## General networking questions
https://www.educba.com/computer-network-interview-questions/


## TCP/IP
https://allabouttesting.org/top-10-interview-questions-tcpudp/

## Explain what happens when you ping 127.0.0.1

## Explain detailed steps of what happens when you google something

# network byte order

https://pythontic.com/modules/socket/byteordering-coversion-functions

Explain why network byte order matters.

# Routing & switching

https://www.guru99.com/ccna-interview-questions.html

## IPv4 vs. IPv6
https://www.techrepublic.com/blog/10-things/10-plus-answers-to-your-questions-about-ipv6/

## DNS

https://sites.google.com/site/vishnuprasadcb/Home/69-dns-interview-questions-answers


## DHCP

https://www.mytectra.com/interview-question/dhcp-interview-questions-and-answers

## VPN

http://networkerinterview.net/entries/vpn/vpn-interview-questions-and-answers

## VLAN & VxLAN

http://tcpipguru.com/vlan-interview-questions/


# firewall

https://allabouttesting.org/top-10-interview-questions-network-firewall/


# ssh

https://www.tecmint.com/ssh-interview-questions/


# security, cryptography


https://resources.infosecinstitute.com/top-30-cryptographer-interview-questions-and-answers-for-2019/#gref

## IPSec

http://tcpipguru.com/ipsec-interview-questions/

## OpenVPN

http://www.ezdevinfo.com/view/openvpn/7221.html


## Compare PPTP, IPSec, OpenVPN, wireguard

https://www.ivpn.net/pptp-vs-ipsec-ikev2-vs-openvpn-vs-wireguard

https://www.ivpn.net/pptp-vs-ipsec-ikev2-vs-openvpn-vs-wireguard

## Crypto agility

https://paragonie.com/blog/2019/10/against-agility-in-cryptography-protocols

## types of linux net devices

https://developers.redhat.com/blog/2018/10/22/introduction-to-linux-interfaces-for-virtual-networking/

* vlan vs vxlan
* macvlan: what is it? what is VEPA, hairpin mode of switches/routers?
* difference between bridge and switch
* ipvlan vs macvlan

## OVN & OVS

https://next.redhat.com/2017/08/15/understanding-the-open-virtual-network/#:~:text=OVN%20is%20a%20system%20to,the%20inner%20workings%20of%20OVN.

# IPv4 and IPv6

* difference in address format and sizes
* differences in other areas: fragmentation, header checksum, SLAAC
* why DHCPv6 is needed at all?



# Storage

https://www.vminstall.com/storage-engineer-skills/

https://www.wisdomjobs.com/e-university/storage-area-network-interview-questions.html


## storage general

Not cloud specific.

https://www.sanfoundry.com/das-nas-san-questions/

http://san-jobs.blogspot.com/2012/01/fc-and-iscsi-san-interview-questions.html


## cloud storage

### What is it?

https://cloud.google.com/storage/docs/introduction


### buckets vs objects

https://cloud.google.com/storage/docs/key-terms


### when is HMAC key useful

https://cloud.google.com/storage/docs/authentication/hmackeys


### EBS

## persistent disk (GCP)


## nfs

https://www.linuxtechi.com/nfs-interview-questions-answers/

## s3

https://www.onlineinterviewquestions.com/aws-s3-interview-questions/

## RAID 

https://mkskistudy.weebly.com/interview-questions-on-raid.html

## LVM

https://www.linvirtshell.com/2017/11/lvm-interview-questions-and-answers.html

## ceph

https://blog.resellerclub.com/what-is-ceph-storage/

## ext2, 3, 4, xfs, btrfs, zfs, ...

https://dev.to/rkeene/btrfs-zfs-and-more-22jg


## iSCSI
https://netappemcstorage.blogspot.com/2016/01/iscsi-questions-answers.html

## netapp
https://mindmajix.com/netapp-interview-questions

## SAN
http://www.tsmtutorials.com/2013/03/san-storage-interview-question-and.html

## CIFS, smb
https://www.linuxforfreshers.com/p/normal-0-false-false-false-en-us-x-none_7.html

## object storage vs. key value

https://en.wikipedia.org/wiki/Object_storage#Differences_between_key-value_and_object_stores

## linux file systems

https://www.sanfoundry.com/linux-questions-file-systems/


## Types of Google cloud storage services

https://cloud.google.com/storage/docs/storage-classes

# Hardware

https://www.hitequest.com/Hardware/El_hardware.htm

https://mindmajix.com/embedded-hardware-design-development-interview-questions

https://www.slajobs.com/hardware-and-networking-interview-questions/

# Desktop Support

https://career.guru99.com/top-50-desktop-support-interview-questions/

# Statistics

https://towardsdatascience.com/12-probability-practice-questions-for-data-science-interviews-2ec5230304d9

https://www.digitalvidya.com/blog/bayesian-statistics-interview-questions-answers/

# Math

https://www.testdome.com/d/math-interview-questions/941

# Bioinformatics

http://biotech.fyicenter.com/resource/Bioinformatics_Interview_Questions_and_Answers.html







