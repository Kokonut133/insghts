# insights
Just a collection of insights, mostly in a professional programming/data science setting

# To checkout

---
# 14.02.2023 Neural Networks: How to enable lifelong learning? (Theory)
- Having an initial structure to embed inputs in a more distinguished form
- Having a central structure using the embedding to allocate processing to subareas of specialization
- Scale the network over time over task to allow areas of specialization drifting of the central general learning structure
- If sufficient scoring is achieved freeze near input areas or gradually decrease plasticity to enable resiliency
- Allocate neurons (=space/resources) according to impact and regularly blank (return to zero signal) unused/mildly ones

# 26.01.2023 Leadership: How to answer questions about your salary?
- often salary is seen as a direct indicator of value -> therefore touchy topic
- if reason to ask is unknown and policies unclear, initially avoid with "Never enough :D"
- talk as a coworker even if you are a department head and be clear about your influence on that decision process
- don't raise hopes before having any confirmation -> crushed hope leads to distrust; an unexpected positive surprise increases trust

# 26.01.2023 Leadership: Quality metrics for Leadership success?
- number of raises you helped pushing
- retention rate of personal
- employees satisfaction
- team productivity velocity

# 26.01.2023 Vision Model: Pretraining: What are good practices working with vision models?
- Vision Transformers seem the go-to in handling and performance (2023)
- Pretraining them via MAE (Masked Auto Encoders) initializes them often very well without the need of labels
- MAE removes randomly 25% of the image and asks to reconstruct the image; supervised task where x and y can be obtained by imagery only

# 17.11.2022 Model Explainability: What can I do to easily get model-agnostic explanations of why a model predicted a way?
- use SHAP
- more specifically: https://github.com/MAIF/shapash
# 17.11.2022 Pipeline Orchestration: What is Pipeline orchestration?
- A tool to create modular, reusable code which can be plugged together in an easy way with a configuration file
# 17.11.2022 Pipeline Orchestration: Which pipeline orchestration should I use at this point?
- Kedro, ZenML, MetaFlow, Airflow are free, popular options
- MetaFlow lacks documentation, flexibility, extensibility; strong interfaces to AWS -> nope
- Kedro is more strict in structuring but has many plugins to enlarge its capabilities
- Kedro is aimed for medium to large teams
- ZenML main strength is its minimalistic nature and integration with many different ML Ops tools
- ZenML allows one to customize more freely ones interactions
- ZenML focuses on small to medium sized teams
- Airflow has a flat learning curve but long-termish is one of the mightiest
- Airflow requires a very specific way of dealing with data
- -> Personal preference is Kedro as enforcement of some minimal standards make it more maintainable overviewable
- -> ZenML if ML Ops parts will change more frequent in the future


# 14.11.2022 Log Tracking: Grafana: What is Grafana?
- a visualization tool for logs, metrics with a time-series nature
# 14.111.2022 MLFlow: What is MLFlow?
- MLFlow is a tool to track experiment metrics, models and serve them
- Ideal for Hyperparameter-tuning?
# 14.11.2022 Models: Decision Trees: How do decision trees learn?
1. Determine metric with highest entropy
2. Find a line to separate based on that feature into classes
3. Inside new split repeat 1-2. until all features gone through
![Decision Tree Splitting](https://www.researchgate.net/publication/342724336/figure/fig2/AS:910463089012746@1594082724852/Decision-tree-data-splitting-This-is-a-revised-figure-taken-from-Zou-Schonlau-17.png)
# 14.11.2022 Model Serving: Nvidia Triton: What is Nvidia Triton?
- Nvidida Triton is a middlepiece focusing on fast inference/prediction model serving and the hardware balancing involved in it
# 14.11.2022 Pipeline Orchestration: Kedro: What is Kedro?
- A modular setup for building, managing, containerizing data science workflows
- includes preprocessing, data versioning, paralellization, requirements handling, visualizations

# 03.11.2022 Agile: What is the Spotify Framework?
- based on Scrum with less formal methods
- central are autonomous groups (squad) that do everything from early development to maintainance
- management focuses on what and why to focus on and engineers try to find the solutions
- details mostly left for the engineers; bigger stuff by management
- low degree of handovers
- chapters are job-title related people
- guilds are cross-group interest structures
![Alignment and Autonomy](https://miro.medium.com/max/720/1*B-0hwMt7gJKo7643fAYyNg.png)
- small frequent releasing with decoupled components; a lot of automated tests, CI/CD
- regular releases (1-3 weeks) including unfinished features that are no activated => see issues arise without exposure


# 02.11.2022 Machine Learning Models: Pruning: What is model pruning and why do it?
- On average model size can be reduced (= Pruning) by 3 to 10 times with less than 10 percent loss in performance
# 02.11.2022 Reading: What is a white paper?
- a simplified paper that focuses on an audience with very little background knowledge
- a how-to/guide/overview
