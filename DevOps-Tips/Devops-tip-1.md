# DevOps Tip 1

When using docker, while testing you may build a lot of images, a good why to clean up the non tagged images is this one:

```
rmi: stand for remove image
-f: stand for filter
-q: stand for quiet, to show only IDS
```
![Devops Tip 1](./img/devops-tip-1.png)