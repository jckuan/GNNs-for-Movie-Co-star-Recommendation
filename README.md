# 2024(Spring)-SMA-Final-Project
## Graph Neural Network for Movie Co-star Recommendation
> *This is a school project for **Social Media Analysis***

Our research focuses on a data-driven approach to recommend movie co-stardom in perspective of profitability. We collected movie and actor data to construct collaboration network, and utilized node embedding (*EGES*, *Node2Vec*) and message passing machanism (*GCN*, *SEAL*) to solve a link prediction task.

For Detail please see *`Graph Neural Network for Movie Co-star Recommendation.pdf`*

Model & Experiments
-----------

We conducted experiments on the collaboration network data of movie actors using
four models, which include:

***1) Baseline model*** (ML-based): only using features of the
two actors and predicting with XGBoost Classifier, 

***2) Benchmark models*** (EGES,
GCN): utilizing actor and network information, 

***3) Best model*** (SEAL): employing a more advanced model architecture for actor collaboration link prediction. 

We used AUC as the model evaluation metric.

|       | ML-based |  EGES  | GCN | SEAL |
|-------|----------|--------|-----|------|
| Valid |   61.1%  |  59.2% | 67.2% | 84.5% |
| Test  |   55.3%  |  59.2% | 67.6% | 80.1% |

Contribution
-----------
| Contributor | Work |
|-------------|------|
| *Jih-Ming Bai* | Problem Formulation, Model, Experiment and Analysis |
| *Cheng-Yu Kuan* | Literature Review, Gradio Demo   |
| *Po-Yen Chu*    | EGES Model and Experiment       |
| *Shang-Qing Su* | Data Collection, Report Delivery |
| *Chia-Shan Li*  | Data Collection, Report Delivery |

