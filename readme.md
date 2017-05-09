# ???
呃，编译electron 1.6 的sqlite版本
直接用目录下编译好的文件也行

# 编译步骤
1. 安装windows本地编译环境
npm install --global --production windows-build-tools

2. 进入sqlite3模块执行编译命令
node-gyp rebuild --target=1.6.6 --arch=x64 --target_platform=win32 --dist-url=https://atom.io/download/electron/ --module_name=node_sqlite3 --module_path=../lib/binding/electron-v1.6-win32-x64

3. 编译完成后会生成 \sqlite3\lib\binding\electron-v1.6-win32-x64\node_sqlite3.node



