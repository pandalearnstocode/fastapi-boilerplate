# Fast API boiler plate

## Setup local environment

```
conda create --name fastapi python=3.8
conda activate fastapi
pip install fastapi
pip install uvicorn[standard]
```

## Run the following command to test things in local

```
cd app
uvicorn main:app --reload
```

## Run the following command to build a run the app

```
docker build -t api .
docker run -d -p 80:80 api
```

## Next step

* build a muli-stage docker build
* change the content of the app
* create a requement file for additional dependencies
* check app in local and in docker
* push docker in registry
* deploy app in cloud component
* check everything is working fine or not
* if everything is working build aCI pipeline (build, push)
* if everything is working build a CD pipeline (deploy)