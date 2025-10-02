# ❄️🐳 Fourth Industrial Systems — Cloud‑Native AI/ML on Kubernetes

Curated by **Fourth Industrial Systems (4th.is)**, this guide highlights open‑source tools and patterns for **AI, Deep Learning, Machine Learning, Computer Vision, Data Science, and Analytics** designed to run **natively on [Kubernetes](http://kubernetes.io/)** and **[Docker](https://www.docker.com/)**. We work across languages — [Python](https://www.anaconda.com/download/), [R](https://mran.microsoft.com/open), [Scala](https://github.com/JetBrains/intellij-scala-bundle), [Java](http://www.oracle.com/technetwork/java/javase/downloads/jdk10-downloads-4416644.html), [C#](https://github.com/dotnet/core), [Go](https://golang.org/), [Julia](https://julialang.org/downloads/), [C++](https://isocpp.org/) — with practical emphasis on **Kubeflow**, **Seldon Core**, **Pachyderm**, **Banzai Pipeline**, **H2O**, **TensorFlow**, **CNTK**, **XGBoost**, **MXNet**, **PyTorch**, **ONNX**, **Argo**, **Airflow**, **Apache Beam**, **Apache Spark**, **Intel BigDL**, **Rook**, and **Ambassador**.

> “The wind and the waves are always on the side of the ablest navigator.” — Edmund Gibbon

---

## Introduction

Across industry, **Kubernetes** has become the standard for orchestrating distributed systems — whether on‑prem, in a single cloud, or spanning many. In contrast, many ML and data workflows still begin on laptops or ad‑hoc notebook servers. This repository shows how to **elevate those experiments into reliable, scalable, reproducible, and portable Kubernetes deployments**.

### Why Kubernetes for ML

- **Elastic scale** for CPU/GPU resources with automated orchestration.  
- **Portability**: the same workloads run across all major clouds and on‑prem.  
- **Ecosystem momentum**: see wide adoption in the [CNCF membership](https://www.cncf.io/about/members/).  
- **Self‑healing**: immutable containers plus controllers enable resilient apps.

### Practical Considerations

- **Containerization**: package apps as small, efficient images for rapid scale‑out.  
- **Immutability**: predictable rollouts, easy rollbacks, and reproducibility.  
- **Persistent storage**: plan PVCs/CSI drivers early; projects like [Rook](https://rook.io) are popular.  
- **Service connectivity**: ephemeral pods change the way services talk; a **service mesh** helps (see <http://layer5.io/service-meshes/>).

---

We focus on **AI/ML/Data Science OSS** that thrives in infinitely scalable Kubernetes environments. For a broader view of orchestration and operations, see **[Awesome Machine Learning Operations](https://github.com/axsauze/awesome-machine-learning-operations)**.

You may also want domain‑specific “awesome” lists:

### Kubernetes
- [awesome-kubernetes](https://github.com/ramitsurana/awesome-kubernetes)  
- [Awesome Helm](https://github.com/cdwv/awesome-helm)  
- [Awesome Operators](https://github.com/operator-framework/awesome-operators)  
- [Awesome Docker](https://github.com/veggiemonk/awesome-docker)  
- [container-security-awesome](https://github.com/kai5263499/container-security-awesome)  
- [Awesome Linux Containers](https://github.com/Friz-zy/awesome-linux-containers)

### Spark
- [Awesome Spark](https://github.com/awesome-spark/awesome-spark)  
- [Awesome Apache Spark Packages](https://github.com/Mageswaran1989/awesome-ApacheSpark-collections)  
- [Awesome Scala](https://github.com/lauris/awesome-scala)

### AI/ML
- [awesome-AIOps](https://github.com/linjinjin123/awesome-AIOps)  
- [Awesome Julia](https://github.com/greister/Awesome-Julia)  
- [Awesome R](https://github.com/qinwf/awesome-R)  
- [Awesome Bioinformatics](https://github.com/shenwei356/awesome/blob/master/bioinformatics.md)  
- [Awesome Recurrent Neural Networks](https://github.com/kjw0612/awesome-rnn)  
- [Awesome Reinforcement Learning](https://github.com/aikorea/awesome-rl)  
- [Awesome Artificial Intelligence](https://github.com/owainlewis/awesome-artificial-intelligence)  
- [Awesome Machine Learning](https://github.com/josephmisiti/awesome-machine-learning)  
- [Awesome StarCraft AI](https://github.com/SKTBrain/awesome-starcraftAI)  
- [Awesome Quantum Machine Learning](https://github.com/krishnakumarsekar/awesome-quantum-machine-learning)  
- [Awesome AI](https://github.com/hades217/awesome-ai)  
- [Awesome Feature Engineering](https://github.com/aikho/awesome-feature-engineering)  
- [Awesome WindowsML ONNX Models](https://github.com/ChangweiZhang/Awesome-WindowsML-ONNX-Models)  
- [Awesome-ONNX-Models](https://github.com/ChangweiZhang/Awesome-ONNX-Models)  
- [Awesome TensorFlow](https://github.com/jtoy/awesome-tensorflow)  
- [Awesome Blockchain AI](https://github.com/steven2358/awesome-blockchain-ai)  
- [Awesome Deep Learning](https://github.com/ChristosChristofidis/awesome-deep-learning)  
- [Awesome Deep Learning Resources](https://github.com/guillaume-chevalier/Awesome-Deep-Learning-Resources)  
- [awesome-nlp](https://github.com/keon/awesome-nlp)  
- [Awesome-Pytorch-list](https://github.com/bharathgs/Awesome-pytorch-list)  
- [awesome-ai-services](https://github.com/sekwiatkowski/awesome-ai-services)  
- [awesome_list_ai_bot_programming](https://github.com/stuffyjumpy/awesome_list_ai_bot_programming)  
- [ML & DL Tutorials](https://github.com/ujjwalkarn/Machine-Learning-Tutorials)  
- [ML on Source Code](https://github.com/src-d/awesome-machine-learning-on-source-code)  
- [ML Interpretability](https://github.com/jphall663/awesome-machine-learning-interpretability)  
- [Interpretable ML](https://github.com/lopusz/awesome-interpretable-machine-learning)  
- [AutoML Papers](https://github.com/hibayesian/awesome-automl-papers)  
- [Awesome H2O](https://github.com/h2oai/awesome-h2o)  
- [Awesome MXNet](https://github.com/chinakook/Awesome-MXNet)  
- [Awesome Bots](https://github.com/hackerkid/bots)  
- [Awesome ChatOps](https://github.com/exAspArk/awesome-chatops)

### Other Data/ETL/Analytics
- [Awesome Apache Airflow](https://github.com/jghoman/awesome-apache-airflow)  
- [Awesome Big Data](https://github.com/onurakpolat/awesome-bigdata)  
- [Awesome-BigData](https://github.com/Harshakvarma/Awesome-BigData)  
- [awesome-datasets](https://github.com/datasciencethgrp/awesome-datasets)  
- [Awesome Analytics](https://github.com/onurakpolat/awesome-analytics)  
- [Awesome Data Science](https://github.com/bulutyazilim/awesome-datascience)  
- [Awesome Pipeline](https://github.com/pditommaso/awesome-pipeline)  
- [Awesome Nextflow](https://github.com/nextflow-io/awesome-nextflow)  
- [awesome-etl](https://github.com/pawl/awesome-etl)  
- [Awesome Business Intelligence](https://github.com/thenaturalist/awesome-business-intelligence)

---

## Community & Attribution

Open‑source projects are maintained by people and teams of all sizes. If you find value here, please **star upstream repos**, file **issues/PRs**, and thank maintainers. If something’s missing, open a discussion and we’ll add it.

---

## Kubernetes — Name & Heritage

*Kubernetes* translates roughly to **“helmsman”** and draws design lineage from Google’s **Borg**. The internal codename *Project Seven* nods to *Seven of Nine* from Star Trek; the logo’s seven spokes reference that origin. More background: <https://en.wikipedia.org/wiki/Kubernetes>.

> “The duties of the ruler are like those of the helmsman of a great ship…” — Han Fei

---

# ML Built for Kubernetes (Native Kube)

> “If you want to build a ship… teach them to yearn for the vast and endless sea.” — Antoine de Saint‑Exupéry

### Kubeflow
<http://kubeflow.org/> — Cloud‑native ML platform.  
- **Training**: TFJob controller for CPU/GPU scaling ([tf-operator](https://github.com/kubeflow/tf-operator)).  
- **Serving**: TensorFlow Serving and integrations with **[Seldon Core](https://www.seldon.io/)**.  
- **Multi‑framework**: operators for **[PyTorch](https://github.com/kubeflow/pytorch-operator)**, **[MXNet](https://github.com/kubeflow/mxnet-operator)**, **Chainer**, with ingress via **[Ambassador](https://www.getambassador.io/)** and pipelines with **[Pachyderm](http://pachyderm.io/)**.

- Extras: **[Kubeflow Labs](https://github.com/Azure/kubeflow-labs)** (Azure), **[H2O + Kubeflow](https://github.com/h2oai/h2o-kubeflow)**.

### Seldon Core
<https://www.seldon.io/> — Kubernetes‑native model serving: <https://github.com/SeldonIO/seldon-core>.

### Pachyderm
<http://pachyderm.io/> — Versioned data pipelines for production ML: <https://github.com/pachyderm/pachyderm>.

### Fabric for Deep Learning (FfDL)
Multi‑framework deep learning on Kubernetes (TensorFlow, Caffe, PyTorch).  
Docs: <https://developer.ibm.com/patterns/deploy-and-use-a-multi-framework-deep-learning-platform-on-kubernetes/>  
Code: <https://github.com/IBM/FfDL>

### Polyaxon
Platform for building, training, and monitoring large‑scale DL apps.  
<https://polyaxon.com/> • <https://github.com/polyaxon/polyaxon>

### Datalayer
Big Data Science on Kubernetes.  
<https://github.com/datalayer/datalayer> • <https://datalayer.io> • <https://docs.datalayer.io>

### IntelAI Machine Learning Container Templates
Accelerators for building ML containers and K8s objects.  
<https://github.com/IntelAI/mlt>

---

# ML Adapted to Kubernetes

> “Impossible is a word humans use far too often.” — Seven of Nine

### Pipeline.AI
Real‑time enterprise AI platform with K8s quickstart:  
<https://github.com/PipelineAI/pipeline> • <https://pipeline.ai>

### Dask & Friends
- **Dask** scales Python for analytics: <https://github.com/dask/dask> • <http://dask.pydata.org/en/latest/>  
  Examples: <https://github.com/dask/dask-examples> • Tutorial: <https://github.com/dask/dask-tutorial>  
- **Dask‑Kubernetes**: <https://github.com/dask/dask-kubernetes> • Docs: <https://dask-kubernetes.readthedocs.io/en/latest/>  
  Helm: <https://github.com/dask/helm-chart> • Docker: <https://github.com/dask/dask-docker>  
- **Dask‑ML**: <https://github.com/dask/dask-ml> • <http://ml.dask.org/>  
- **Dask‑XGBoost**: <https://github.com/dask/dask-xgboost>

### Kafka on K8s (Helm)
<https://github.com/Landoop/kafka-helm-charts> • Connectors: <https://github.com/Landoop/stream-reactor>

### Big Data Playground
End‑to‑end sample stack (K8s, Spark/Flink/Beam, Kafka, etc.):  
<https://github.com/Chabane/bigdata-playground>

---

# Pipeline & Data Flow

### Banzai Pipeline
From commit to scale on Kubernetes (CI/CD, logging, monitoring, autoscaling):  
<https://github.com/banzaicloud/pipeline>

### Argo
Container‑native workflows; cloud‑agnostic; runs on any Kubernetes cluster:  
<https://argoproj.github.io/> • <https://github.com/argoproj/argo>  
Events: <https://github.com/argoproj/argo-events>

### Apache Airflow
Author, schedule, and monitor DAGs for ETL/ML: <https://airflow.apache.org/>  
Best practices: <https://gtoonstra.github.io/etl-with-airflow/>  
K8s tools: <https://github.com/mumoshu/kube-airflow> • Operator: <https://github.com/GoogleCloudPlatform/airflow-operator>

### Apache Beam / Dataflow
- **Beam Operator**: <https://github.com/aleksdjuricin/beam-operator>  
- **Cron‑scheduled Beam Jobs**: <https://github.com/sanderploegsma/beam-scheduling-kubernetes>  
- **Google Cloud Dataflow Templates**: <https://github.com/GoogleCloudPlatform/DataflowTemplates>

---

# Storage for Kubernetes

### Rook
Cloud‑native storage orchestration: <https://rook.io/> • <https://github.com/rook/rook>

### OpenEBS
Container‑attached block storage (Go), with SLAs, tiering, and multi‑AZ replica policies:  
<https://www.openebs.io/> • <https://github.com/openebs/openebs>  
Maya orchestration: <https://github.com/openebs/maya> • Helm: <https://github.com/openebs/charts>

---

# Spark at Sea (on K8s)

> “Only those who brave its dangers comprehend its mystery.” — Longfellow  
> T.S. Eliot, *The Waste Land* (for perspective).

**Note:** Native K8s support arrived in Spark 2.3 and has matured since, but always check your target version’s capabilities.

- **Spark Operator**: <https://github.com/GoogleCloudPlatform/spark-on-k8s-operator>  
- **Spark on PKS (multi‑cloud)**: <https://github.com/SnappyDataInc/spark-on-k8s>  
- **Sparknetes**: <https://github.com/hypnosapos/sparknetes>  
- **HDFS on K8s (Helm charts)**: <https://github.com/apache-spark-on-k8s/kubernetes-HDFS>  
- **Stable Helm chart (Spark)**: <https://github.com/helm/charts/tree/master/stable/spark>  
- **Helm chart (Spark Operator)**: <https://github.com/helm/charts/tree/master/incubator/sparkoperator>  
- **Kubernetes examples** (Spark): <https://github.com/kubernetes/examples/tree/master/staging/spark> (may be out of date)

### Intel BigDL & Analytics Zoo
- **BigDL**: <https://bigdl-project.github.io/> • <https://github.com/intel-analytics/BigDL>  
  - Core: <https://github.com/intel-analytics/BigDL-core>  
  - Getting Started: <https://bigdl-project.github.io/master/#getting-started/>  
  - Tutorials: <https://github.com/intel-analytics/BigDL-tutorials>  
  - Workshops: <https://github.com/alex-kalinin/lenet-bigdl>  
- **Analytics Zoo**: <https://analytics-zoo.github.io/> • <https://github.com/intel-analytics/analytics-zoo>

---

# Spark on OKD / OpenShift

- **Rad Analytics Spark Operator**: <https://github.com/radanalyticsio/spark-operator>  
- **OpenShift Spark Images**: <https://github.com/radanalyticsio/openshift-spark>  
- **SparkPi (Vert.x) tutorial**: <https://github.com/radanalyticsio/tutorial-sparkpi-java-vertx>

---

# Utilities & Accessories

- **EFK (Elastic/Fluentd/Kibana) Helm**: <https://github.com/cdwv/efk-stack-helm>  
- **Draft** (Azure): <https://draft.sh/> • <https://github.com/Azure/draft>  
  Pack repo plugin: <https://github.com/draftcreate/draft-pack-repo>  
- **Brigade** (event‑driven pipelines): <https://brigade.sh/> • <https://github.com/Azure/brigade>  
  - Dashboard: <https://github.com/Azure/kashti>  
  - Terminal UI: <https://github.com/slok/brigadeterm>  
  - Prometheus exporter: <https://github.com/slok/brigade-exporter>  
  - Gateways: BitBucket, GitLab, K8s events, Event Grid, Cron, Trello  
  - Build your own gateway: <https://github.com/technosophos/draft-brigade>  
- **ksonnet** (historical): <https://ksonnet.io/>

---

## Odds & Ends

The **podder‑ai** ecosystem offers related components:  
- **Kubeb** (CLI for building/deploying to K8s): <https://github.com/podder-ai/kubeb>  
- **pipeline‑framework** (Airflow‑based scheduling/monitoring): <https://github.com/podder-ai/pipeline-framework>  
- **pipeline‑generator** and sample repos:  
  <https://github.com/podder-ai/pipeline-generator> •  
  <https://github.com/podder-ai/pipeline-framework-sample> •  
  <https://github.com/podder-ai/poc-base-sample> •  
  <https://github.com/podder-ai/poc-base>

---

### About Fourth Industrial Systems

**Fourth Industrial Systems** builds scalable, ethical AI solutions and agentic workflows that move seamlessly from **prototype to production** on Kubernetes.  
Contact: **freeman@4th.is** • Learn: **learn.4th.is** • News: **news.4th.is**

**Trademarks**: Kubernetes®, Apache®, NVIDIA®, and other names are the property of their respective owners; references are for identification only and imply no endorsement.
