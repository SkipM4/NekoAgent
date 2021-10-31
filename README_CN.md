# NekoAgent

## 一个旨在为Paper系服务端核心提供部分特性自定义的项目

## 特性

- 允许末地传送门刷沙机制.
- 禁止末地黑曜石柱生成.
- 禁止末地黑曜石平台生成.
- 允许切石机对玩家等实体造成伤害.
- 允许潜影贝在末地城内生成.
- 允许玩家使用栓绳牵引村民.
- 向玩家发送虚假的权限等级为4数据包.
- 可使用 `/mspt <ms>` 指令修改服务器TPS值.
- 修改服务端核心名（支持§字符与RGB颜色）.

## 用法

```bash
java -javaagent:NekoAgent.jar=附加参数 -jar 服务端核心.jar
```
#### 如

```bash
java -javaagent:NekoAgent-1.0-SNAPSHOT.jar=enableSandDuplication -jar paper-1.17.1-353.jar
java -javaagent:NekoAgent-1.0-SNAPSHOT.jar=disableObsidianSpikesReset -jar purpur-1.17.1-1421.jar
java -javaagent:NekoAgent-1.0-SNAPSHOT.jar=enableStoneCutterDamage+enableShulkerSpawningInEndCities -jar tuinity-paperclip.jar
```

## 可用参数

- enableSandDuplication
- disableObsidianSpikesReset
- enableStoneCutterDamage
- enableShulkerSpawningInEndCities
- enableLeashableViallagers
- enableSetMSPTCommand
- enableFakePermissionLevel4
- maxShulkersCount=4
- minShulkersCount=1

## 构建

```bash
gradlew build
```

## 贡献者

Shirasawa huzpsb SkipM4

## 许可证

[MIT](./LICENSE)
