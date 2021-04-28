# docker-whistle

将 WhistleAppData 复制出来

```
docker cp whistle:~/.WhistleAppData ~/.WhistleAppData
```

```
docker run --rm -p 8899:8899 -v .WhistleAppData:~/.WhistleAppData 0x1f/whistle w2 run
```

后台运行

```
docker run -d --rm -p 8899:8899 -v .WhistleAppData:~/.WhistleAppData 0x1f/whistle w2 start
```