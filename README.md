# SpringBootConcoursePipeline

this pipeline is used to take the code from git and it considers maven docker image as base image and runs maven application and then it will deploy the app to PCF using concourse pipeline

fly set-pipeline --target lite --config ci/pipeline.yml --pipeline spring-app --non-interactive --load-vars-from credentials.yml

