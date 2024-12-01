config through kubectl cmd

kubectl create configmap <config-name> --from-literal=app-name=MyApp --from-literal=log-level=DEBUG

kubectl create configmap file-config --from-file=config.json 
    to apply this cmd we need to create one file with config.json name 

kubectl create configmap multi-file-config --from-file=app.properties --from-file=database.properties

kubectl create configmap directory-config --from-file=/path/to/config-directory/
    if there are multiple files with in a directory then we can give path to directory only.