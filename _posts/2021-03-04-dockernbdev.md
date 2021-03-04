
# nbdeb with Docker
## docker命令
### 查看本地镜像
```
~> docker images                            
REPOSITORY            TAG       IMAGE ID       CREATED       SIZE
fastdotai/nbdev-dev   latest    f37f83e5f8a6   3 weeks ago   2.11GB
```
### 建镜像并挂本地目录

`~> docker run -it -v /Users/liguimei/Documents/dockerlocal:/home/local fastdotai/nbdev-dev /bin/bash`

### 将nbs内的ipynb文件拷贝到local文件夹
```
runner@f566539e687c:~/cp nbs/*.ipynb local/
runner@f566539e687c:~$ cd local
runner@f566539e687c:~/local$ ls
00_export.ipynb       05_merge.ipynb   index.ipynb
01_sync.ipynb         06_cli.ipynb     tutorial_colab.ipynb
02_showdoc.ipynb      07_clean.ipynb   tutorial.ipynb
03_export2html.ipynb  99_search.ipynb
04_test.ipynb         example.ipynb
```

