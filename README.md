## c++11 
尽量全用c++11标准和google stype，除了一些和cuda冲突的地方。

## 依赖
金莲减少外部安装依赖，最好是编译即可使用。

## 编译
 - 支持GPU可选编译
 - 对于CPU模式，支持跨平台（linux, window, mac, android, ios）
 - 对于GPU模式，目前只支持linux即可（建议开发人员都用linux）
 - CPU可用的核数和GPU可用的卡数不必相关
 - 支持层可选编译
 - 使用bazel进行编译管理

## 多级多卡
 - 打开GPU开关时默认支持多级多卡
 - 使用mpi进行并行通信（目前没有发现更优雅地方式）
 - 在solve中控制每个层的并行模式？
 - 支持数据并行和模型并行？
