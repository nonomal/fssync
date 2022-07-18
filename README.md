<p align='center'>
  <pre style="float:left;">
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

<p align='center'>
方便地<sup><em>FsSync</em></sup> 文件同步工具
<br> 
</p>

<br>

## 背景

大文件同步工具，包括服务端与客户端工具

基于tus分片协议

## 特性

- 🗂 服务端
- 📦 客户端

## 使用手册
### 安装

```bash
go install github.com/wwqdrh/fssync@latest

fssync --help


fssync server --extra [路径]

fssync client download --host [远程路径] --url [下载url] --filename [下载文件名] --spec [分片信息保存路径]
```
