# Prophecy (previously RefreshML)
Automated machine learning training and serving.


# Quickstart:
 install docker and docker-compose - https://docs.docker.com/compose/install/#prerequisites

 run docker-compose -f docker-compose-ab.yaml up

this will download docker images from Dockerhub, and start all services.
Then, go to http://localhost:4200/ to access Dashboard.

# Capabilities:
1) Deploy scikit-learn classifier as a REST api with no coding needed. 
Just upload pickle file with trained model (http://scikit-learn.org/stable/modules/model_persistence.html) to the dashboard or use one trained with AutoML on top of TPOT framework (https://automl.info/tpot/) and send requests.

2) Run A/B testing of models - split traffic accross models for canary deployment.
Send business metric of model performance from your client app (such as successfull clicks on suggestion or false positive, example in https://github.com/deniskovalenko/refreshml-client) 

# Building from source
 Angular Dashboard - https://github.com/deniskovalenko/datascience-dashboard
 
 (optional) AutoML trainer - https://github.com/deniskovalenko/prophecy-trainer
 
 decision-making service - https://github.com/deniskovalenko/brain-server
 
 Client app exposing REST API for models - https://github.com/deniskovalenko/ml-service-backend
 
  

# Features roadmap:
- project workspaces (deploy models for different ML tasks) 
- persistance layer 
- generation of swagger documentation for each machine learning task project
- API token support
- security issues (run apps in separate network and expose ports only of rest endpoint and dashboard)
- support for Kubernetes deployment

# Contributing 
Pull requests are welcome, as well as feature requests and suggestions

# License
Prophecy is dual-licensed under the GNU Affero General Public License (AGPL) version 3.0, and a commercial license.
