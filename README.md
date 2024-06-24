# XRayR-Docker-dev
A Xray backend framework that can easily support many panels.

一个基于Xray的后端框架，支持V2ay,Trojan,Shadowsocks协议，极易扩展，支持多面板对接

Find the source code here: [XrayR-project/XrayR](https://github.com/XrayR-project/XrayR)

# 详细使用教程

[教程](https://xrayr-project.github.io/XrayR-doc/)

## 免责声明

本项目只是本人个人学习开发并维护，本人不保证任何可用性，也不对使用本软件造成的任何后果负责。

## 特点

* 永久开源且免费。
* 支持V2ray，Trojan， Shadowsocks多种协议。
* 支持Vless和XTLS等新特性。
* 支持单实例对接多面板、多节点，无需重复启动。
* 支持限制在线IP
* 支持节点端口级别、用户级别限速。
* 配置简单明了。
* 修改配置自动重启实例。
* 方便编译和升级，可以快速更新核心版本， 支持Xray-core新特性。

## 功能介绍

| 功能        | vmess | vless | trojan | shadowsocks |
|-----------|-------|-------|--------|-------------|
| 获取节点信息| √ | √ | √ |√ |
| 获取用户信息| √ | √ | √ |√ |
| 用户流量统计| √ | √ | √ |√ |
| 服务器信息上报| √ | √ | √ |√ |
| 自动申请tls证书| √ | √ | √ |√ |
| 自动续签tls证书| √ | √ | √ |√ |
| 在线人数统计| √ | √ | √ |√ |
| 在线用户限制| √ | √ | √ |√ |
| 审计规则| √ | √ | √ |√ |
| 节点端口限速| √ | √ | √ |√ |
| 按照用户限速| √ | √ | √ |√ |
| 自定义DNS| √ | √ | √ |√ |

## 支持前端


| 前端                                                     | vmess | vless | trojan | shadowsocks |
|--------------------------------------------------------|-------|-------|--------|-------------------------|
| sspanel-uim                                            | √     | √     | √      | √ (单端口多用户和V2ray-Plugin) |
| v2board                                                | √     | √     | √      | √                       |
| [PMPanel](https://github.com/ByteInternetHK/PMPanel)   | √     | √     | √      | √                       |
| [ProxyPanel](https://github.com/ProxyPanel/ProxyPanel) | √     | √     | √      | √                       |
| [WHMCS (V2RaySocks)](https://v2raysocks.doxtex.com/)   | √     | √     | √      | √                       |
| [GoV2Panel](https://github.com/pingProMax/gov2panel)   | √     | √     | √      | √                       |
| [BunPanel](https://github.com/pennyMorant/bunpanel-release)   | √     | √     | √      | √                       |

## 软件安装



# Docker compose 安装
0. 安装docker-compose: 
```
1.git clone https://github.com/XrayR-project/XrayR-release
2.cd XrayR-release
3.编辑配置文件：config.yml，详见：配置文件说明
4.启动docker：docker-compose up -d

