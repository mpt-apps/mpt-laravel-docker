# mpt-laravel-docker
Docker with nginx, laravel and elasticsearch

### Running

* Clone this repo
```
git clone https://github.com/mpt-apps/mpt-laravel-docker.git
```

* Create 3 folders
```
cd mpt-laravel-docker 
mkdir code
mkdir data
mkdir logs
```

* Create folder to elasticsearch data
```
cd data
mkdir elastic
```

* Load your laravel project: Save your laravel project in ```mpt-laravel-docker/code/mpt-laravel```

* Run docker. Go to ```mpt-laravel``` and run it.
```
docker-compose up 
```
If there is a error about max_map_count, before docker-compose up, you must do
```
sysctl -w vm.max_map_count=262144
```
