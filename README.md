This repository contains a docker environment for a local [MapService](https://github.com/hulop/MapService) server

## data

```
./server_data/
             /attachments
             /MapData.geojson
             /server.env       # check the file for configuration
```


## usage

- launch server (it automatically load the data from server_data dir)
  ```
  ./server-launch.sh
  ```
- access [http://localhost:9090/map/editor.jsp](http://localhost:9090/map/editor.jsp)
  - user/pass = editor/editor
- when you kill the script, server will stop and database will be discarded, so you need to export edited data to save

## required software

- docker
- docker-compose

## tested environment

- Ubuntu20.04
- MacOS14.5

