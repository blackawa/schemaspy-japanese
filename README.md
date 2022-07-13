# Schemaspyを使ったER図生成

## 前提条件

- Dockerがインストールされている

## 使い方

    $ docker build . -t schemaspy/schemaspy:japanese
    $ docker run --rm --add-host=gateway.docker.internal:host-gateway -v "$(PWD)/output:/output" -v "$(PWD)/schemaspy.properties:/schemaspy.properties" schemaspy/schemaspy:japanese -font ipaexg
