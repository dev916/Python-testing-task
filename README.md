# python-testing-task
Python Testing job for Interview.

Test Details:
 
Create an elasticsearch node (docker, local, remote, can be anything), create 3 indices with names project_1 project_2 project_3 then write a python script to reindex all indices matching wildcard `project_*` using Elasticsearch Task management API, then update all documents with last_updated field using Task management API. Hint: task management API allows you to execute tasks without waiting for them.
 
Deliverables:
Python script for initial data ingestion and indices creation
Python script with reindex and update functionality

Possible task for extra points:
Create a small web app to ingest documents to Elasticsearch with POST request. Example:
curl --header "Content-Type: application/json" \
 --request POST \
 --data '{"index":"project_1","payload": {"test": true}}' \
 http://localhost:3000/ingest
