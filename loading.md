#### 加载问题

1. 先看是什么库找不到
```
ldd cephfs.so
```

2. 再看库依赖库查找路径RPATH是否没有包含
```
readelf -d cephfs.so
```

3. 如果需要查看ELF中的符号问题用nm
```
nm cephfs.so  | grep openv
```