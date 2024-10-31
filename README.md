This repository contains a docker environment for a local [MapService](https://github.com/hulop/MapService) server

## data

```
./server_data/
             /attachments
             /MapData.geojson
             /server.env       # check the file for configuration (map center coordinates, etc.)
```


## usage

- launch server (it automatically load the data from server_data dir)
  ```
  ./server-launch.sh -d server_data                     # for localhost access only
  ./server-launch.sh -d server_data -P <port number>    # for public access (be careful)
  ./server-launch.sh -h                                 # to see help
  ```
- access [http://localhost:9090/map/editor.jsp](http://localhost:9090/map/editor.jsp)
  - user/pass = editor/editor
- when you kill the script, server will stop and database will be discarded, so you need to export edited data to save

## required software

- docker

## tested environment

- Ubuntu20.04
- MacOS14.5

