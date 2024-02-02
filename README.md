# Armbian / 岸边 

## 安装及升级 Armbian 的相关说明

选择和你的盒子型号对应的 Armbian 系统，不同设备的使用方法查看对应的说明。

- ### 安装 Armbian 到 EMMC

```shell
armbian-install
```

- ### 更新 Armbian 内核

登录 Armbian 系统 → 输入命令：

```shell
# 使用 root 用户运行 (sudo -i)
# 如果不指定参数，将更新为最新版本。
armbian-update
```

举例: `armbian-update -k 5.15.50 -u dev`

通过 `-k` 参数指定内核版本号时，可以准确指定具体版本号，例如：`armbian-update -k 5.15.50`，也可以模糊指定到内核系列，例如：`armbian-update -k 5.15`，当模糊指定时将自动使用指定系列的最新版本。

- ### 安装常用软件

登录 Armbian 系统 → 输入命令：

```shell
armbian-software
```

- ### 修改 Armbian 配置

登录 Armbian 系统 → 输入命令：

```shell
armbian-config
```
