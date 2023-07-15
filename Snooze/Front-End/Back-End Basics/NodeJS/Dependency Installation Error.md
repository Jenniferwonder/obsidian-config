---
Title: Dependency Installation Error
tags: TechSkills
DateStarted: 2023-02-17
DateModified: 2023-02-17
status:
sr-due: 2023-07-02
sr-interval: 4
sr-ease: 270
---

#### 1. parsing error: cannot find module '@babel/preset-env'

- [[VS Code 安装包解析报错解决思路与方法]]

#### 2. 安装依赖方案 For Windows：

✅Using win cmd> While installing `npm i`, hit

- 🐛bug 1. [reactjs - Could not resolve dependency error peer react@"^16.8.0 || ^17.0.0" from @material-ui/core@4.12.4 - Stack Overflow](https://stackoverflow.com/questions/72596908/could-not-resolve-dependency-error-peer-react16-8-0-17-0-0-from-materia)
- `npm config set legacy-peer-deps true`

#### 3. 安装依赖方案二 For Ubuntu：

✅Trying to use Ubuntu in VSCode to run `npm i`

- 🐛bug 1 again, the same solution as above.
- 🐛bug 2. [dependencies - Npm can't find module "semver" error in Ubuntu 19.04 - Ask Ubuntu](https://askubuntu.com/questions/1152570/npm-cant-find-module-semver-error-in-ubuntu-19-04)
- Reference1: [dependencies - Npm can't find module "semver" error in Ubuntu 19.04 - Ask Ubuntu](https://askubuntu.com/questions/1152570/npm-cant-find-module-semver-error-in-ubuntu-19-04)
- [node.js - How to install node.tar.xz file in linux - Stack Overflow](https://stackoverflow.com/questions/63312642/how-to-install-node-tar-xz-file-in-linux)
- Reference2: **Download Node for Ubuntu** [Set up Node.js on WSL 2 | Microsoft Learn](https://learn.microsoft.com/en-us/windows/dev-environment/javascript/nodejs-on-wsl)
- 🐛bug 3. Trying to download `nvm` using `curl` (curl: (6) Could not resolve host ...)
  - ![[zz-assets/Pasted image 20230217161454.png]]
  - Solution:
  - 1.  Open /etc/hosts with [[vim]]: `sudo vim /etc/hosts`
  - 2.  Find CDN, IP Address for the host [ipaddress.com](https://www.ipaddress.com/ip-lookup)
  - 3.  Insert the IP Address and hostname in [[vim]]
  - 4.  `ping <hostname>` to check successful connection
  - Reference: [Could not resolve host: github.com 的解决方案\_yjn18021006815 的博客-CSDN 博客](https://blog.csdn.net/yjn18021006815/article/details/118568048?spm=1001.2101.3001.6650.3&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EOPENSEARCH%7ERate-3-118568048-blog-57566709.pc_relevant_3mothn_strategy_and_data_recovery&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EOPENSEARCH%7ERate-3-118568048-blog-57566709.pc_relevant_3mothn_strategy_and_data_recovery&utm_relevant_index=4)
