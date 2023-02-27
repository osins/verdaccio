### 启动docker服务
```
docker-compose up -d
```

### 添加登录用户

### step1 本地安装 verdaccio-htpasswd
```
npm install -g verdaccio-htpasswd
```

### step2 添加用户 (http://localhost:4873更改为你远程私有仓库的地址)
```
npm adduser --registry http://localhost:4873
```

### 添加依赖
```
npm install -g nrm
nrm add dnpm http://localhost:4873
nrm use dnpm
nrm test dnpm
npm login
```