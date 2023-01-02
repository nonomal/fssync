<div align="center">
  <p>
      <pre style="float:center">
              .-')      .-')                      .-') _              
             ( OO ).   ( OO ).                   ( OO ) )             
   ,------. (_)---\_) (_)---\_)   ,--.   ,--.,--./ ,--,'     .-----.  
('-| _.---' /    _ |  /    _ |     \  `.'  / |   \ |  |\    '  .--./  
(OO|(_\     \  :` `.  \  :` `.   .-')     /  |    \|  | )   |  |('-.  
/  |  '--.   '..`''.)  '..`''.) (OO  \   /   |  .     |/   /_) |OO  ) 
\_)|  .--'  .-._)   \ .-._)   \  |   /  /\_  |  |\    |    ||  |`-'|  
  \|  |_)   \       / \       /  `-./  /.__) |  | \   |   (_'  '--'\  
   `--'      `-----'   `-----'     `--'      `--'  `--'      `-----'  
  </pre>
  </p>
  <p>

  <p align='center'>
方便地<sup><em>FsSync</em></sup> 文件同步工具
<br> 
</p>


[![Build Status](https://github.com/wwqdrh/fssync/actions/workflows/push.yml/badge.svg)](https://github.com/wwqdrh/fssync/actions)
[![codecov](https://codecov.io/gh/wwqdrh/fssync/branch/main/graph/badge.svg?token=0QUPXM08Z1)](https://codecov.io/gh/wwqdrh/fssync)

  </p>
</div>


## 背景

大文件同步工具，包括服务端与客户端工具

基于tus分片协议

## 特性

- 🗂 服务端
- 📦 客户端

## 使用手册

### 注意事项

- 使用相对路径作为参数
- 客户端在下载文件的时候，无论是对于需要分片的大文件还是小文件都需要经过filespec获取分片信息以及filetrunc下载对应分片两步

### 安装

```bash
go install github.com/wwqdrh/fssync@latest

fssync --help
```

### 使用

操作界面为tui，根据提示填写必要参数即可

```bash
fssync -mode server

fssync -mode client
```

拉取服务端的文件夹, 默认同步时间间隔为10秒

```bash
fssync server -d [需要开放的文件夹]

fssync client download -h [服务端地址] --watch --all
```