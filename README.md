# Graph Neural Network for Movie Co-star Recommendation

[**[paper]**](https://drive.google.com/file/d/1IgunKXLMQ79FNa_EPTB9jD0qhMjMNF9f/view?usp=drive_link) | [**[slides]**](https://drive.google.com/file/d/1iwTejAxF8fyCZaaDBvE6iDzNs33SaQI1/view?usp=drive_link)

Our research takes a data-driven approach to recommend co-starring in a movie. We collected movie and actor data from multiple sources to construct a network, and utilized node embeddings (*EGES*, *Node2Vec*) and message passing machanisms (*GCN*, *SEAL*) to solve a link prediction task.

## Models & Experiments

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

## Empirical Results

Below are some examples shown on a Gradio interface.
![Expected output]()

## Contribution

| Contributor | Work |
|-------------|------|
| *Jih-Ming Bai* | Problem Formulation, Model, Experiment and Analysis |
| *Cheng-Yu Kuan* | Literature Review, Gradio Demo   |
| *Po-Yen Chu*    | EGES Model and Experiment       |
| *Shang-Qing Su* | Data Collection, Report Delivery |
| *Chia-Shan Li*  | Data Collection, Report Delivery |

