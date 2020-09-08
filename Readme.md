# NPM-Cache

This project stores cahce for offline npm installation


## Online Machine

### 2020-09-04

```bash
npm install -g @angular/cli
mkdir /workspace/npm-cache/npm_cache
ng new ng-npm-cache --skip-install --skip-git
cd ng-npm-cache
npm install --online --cache=/workspace/npm-cache/npm_cache
npm install @angular/material@10.2.0 --online --cache=/workspace/npm-cache/npm_cache
npm install @angular/cdk@10.2.0 --online --cache=/workspace/npm-cache/npm_cache
npm install @tensorflow/tfjs --online --cache=/workspace/npm-cache/npm_cache
npm install pkg --online --cache=/workspace/npm-cache/npm_cache
npm install javascript-lp-solver --online --cache=/workspace/npm-cache/npm_cache
```

### 2020-09-08

```bash
cd ng-npm-cache
npm install material-design-icons --online --cache=/workspace/npm-cache/npm-cache-0908
npm install http-server --online --cache=/workspace/npm-cache/npm-cache-0908
```

### 2020-09-08-01

```bash
cd ng-npm-cache
npm install mxgraph --online --cache=/workspace/npm-cache/npm-cache-0908-1
npm install @angular/pwa --online --cache=/workspace/npm-cache/npm-cache-0908-1
```

## Offline Machine

Copy /workspace/npm-cache/npm_cache to "D:\\bin\\npm_cache"

```bash
npm config set prefer-offline true
npm config set cache "D:\\bin\\npm_cache"
npm install --offline -g @angular/cli
```

## Reference

[完全離線安裝npm套件](https://blog.miniasp.com/post/2018/06/16/Offline-installation-of-npm-packages-for-Enterprise)
