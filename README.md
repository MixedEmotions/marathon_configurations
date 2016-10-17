# Marathon Configurations
In this repository you will find Marathon configuration files for the different MixedEmotions modules that you can find in MixedEmotions' Dockerhub (https://hub.docker.com/u/mixedemotions/).

These configurations were tested using Marathon 0.10.1, depending on your version, operation or configuration files might vary slightly.

For uploading one of these configurations, it is only needed to make a POST request to your Marathon installation. Example:

     curl -X POST -H 'Content-Type: application/json' localhost:8080/v2/apps --data @selected_file.json

