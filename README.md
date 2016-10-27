# Marathon Configurations
In this repository you will find Marathon configuration files for the different MixedEmotions modules that you can find in MixedEmotions' Dockerhub (https://hub.docker.com/u/mixedemotions/).

These configurations were tested using Marathon 0.10.1, depending on your version, operation or configuration files might vary slightly.

For uploading one of these configurations, it is only needed to make a POST request to your Marathon installation. Example:

     curl -X POST -H 'Content-Type: application/json' localhost:8080/v2/apps --data @selected_file.json

Available configurations

* 06_audioanalysis_up.json (https://hub.docker.com/r/mixedemotions/06_audioanalysis_up/)
* 08_spanish_entity_extraction.json (https://hub.docker.com/r/mixedemotions/08_entity_extraction_pt/)
* 13_spanish_topics.json (https://hub.docker.com/r/mixedemotions/13_topic_extraction_spanish/)
