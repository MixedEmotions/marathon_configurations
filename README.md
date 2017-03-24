# Marathon Configurations
In this repository you will find Marathon configuration files for the different MixedEmotions modules that you can find in MixedEmotions' Dockerhub (https://hub.docker.com/u/mixedemotions/).

These configurations were tested using Marathon 0.10.1, depending on your version, operation or configuration files might vary slightly.

For uploading one of these configurations, it is only needed to make a POST request to your Marathon installation. Example:

     curl -X POST -H 'Content-Type: application/json' localhost:8080/v2/apps --data @selected_file.json

Available configurations

* 06_audioanalysis_up.json (https://hub.docker.com/r/mixedemotions/06_audioanalysis_up/)
* 08_spanish_entity_extraction.json (https://hub.docker.com/r/mixedemotions/08_entity_extraction_pt/)
* 10_entity_linking_nuig.json (https://hub.docker.com/r//mixedemotions/10_entity_linking_nuig)
* 13_spanish_topics.json (https://hub.docker.com/r/mixedemotions/13_topic_extraction_spanish/)

## Troubleshooting

Some of the docker images are large and [exceed the default MESOS timeouts when loading](https://github.com/MixedEmotions/MixedEmotions/wiki/Installation-Manual#docker-in-mesos). This can be fixed with the following configuration:

    export MESOS_execution_registration_timeout=5mins



## Acknowledgement

This module was developed by [Paradigma Digital](https://en.paradigmadigital.com/) as part of the MixedEmotions project. This development has been partially funded by the European Union through the MixedEmotions Project (project number H2020 655632), as part of the `RIA ICT 15 Big data and Open Data Innovation and take-up` programme.

![MixedEmotions](https://raw.githubusercontent.com/MixedEmotions/MixedEmotions/master/img/me.png) 

![EU](https://raw.githubusercontent.com/MixedEmotions/MixedEmotions/master/img/H2020-Web.png)

 http://ec.europa.eu/research/participants/portal/desktop/en/opportunities/index.html
