<h1 align="center">
  <br>
  <img src="https://raw.githubusercontent.com/GoMinerProxy/GoMinerProxy/main/images/logo.png" width="350"/>
</h1>

<h4 align="center">基於GoLang的高性能多線程ETH礦池轉發中繼代理工具. </h4>

<p align="center">
  <a>
    <img src="https://img.shields.io/badge/language-golang-green.svg" alt="travis">
  </a>
  <a>
    <img src="https://img.shields.io/badge/release-1.0.5-orgin.svg" alt="travis">
  </a>
  <a>
    <img src="https://img.shields.io/badge/license-apache-orgin.svg" alt="travis">
  </a>
</p>

<p align="center">
  <a href="https://github.com/GoMinerProxy/GoMinerProxy/blob/main/README_zh-cn.md">简体介绍</a> •
  <a href="https://gominerproxy.github.io/zh_hk/">文檔(繁體中文)</a> •
  <a href="https://gominerproxy.github.io/zh_cn/">文档(简体中文)</a> •
  <a href="https://t.me/+afVqEXnxtQAyNWNh">Telegram 討論群组</a> •
  <a href="https://t.me/go_minerproxy">Telegram 通知頻道</a>
</p>

## :sparkles: 特性

* :cloud: 礦池轉發：支持ETH的中繼代理，方便統一管理 (BTC/ETC/LTC等即将更新)
* :zap: 超高性能：採用高效率的GoLang語言編寫，並對多線程進行優化
* 💻 自定義抽水：支持中繼平台自定義抽水比例進行抽水，方便賺取服務器維護成本
* 📚 多種抽水算法：用戶可自選各種抽水算法，防止算力出現週期函數或心跳圖的情況
* 💾 安全穩定：支持TCP、SSL等方式，並對CC攻擊編寫一定的策略進行防護
* :outbox_tray: 批量轉發：一個軟件即可開啟對多個礦池的轉發，無需開啟多個進程
* :card_file_box: 熱修改：配置均可網頁後台上熱修改，無需再修改繁瑣配置文件再重啟
* :art: 精美後台：後台網頁功能全面、統計豐富、黑暗模式、多語言支持
* :eye_speech_bubble: 完善社區支持：Telegram 群組內可幫助處理解決遇到的各類問題，歡迎提出反饋建議
* :rocket: 開箱即用：All-In-One 打包，一鍵搭建運行，一鍵配置
* :family_woman_girl_boy: 多系統支持：Windows Linux MacOS均可支持使用，無需額外環境等
* :gear: 專業團隊：擁有豐富區塊鏈開發的工作經驗，多名開發人員來自香港科技大學名校
* :link: 分佈式系統(後續更新)
* 🌈 ... ...

## :hammer_and_wrench: 部署

最新軟件版本請見：<a href="https://github.com/GoMinerProxy/GoMinerProxy/releases">Github Release</a></br>
Windows 直接下載適用於您目標機器操作系統、CPU架構的主程序，直接運行即可。<a href="https://gominerproxy.github.io/zh_hk/1%20-%20%E5%BF%AB%E9%80%9F%E9%96%8B%E5%A7%8B/1.1%20-%20Windows%E7%B3%BB%E7%B5%B1.html">Windows詳細教程</a>
</br>
Linux 可按照下述指令運行，請注意下載鏈接需要適用於您目標機器操作系統、CPU架構。<a href="https://gominerproxy.github.io/zh_hk/1%20-%20%E5%BF%AB%E9%80%9F%E9%96%8B%E5%A7%8B/1.2%20-%20Linux%E7%B3%BB%E7%B5%B1.html">Linux詳細教程</a>

### Linux一鍵脚本
```shell
# 先安装curl/wget/screen软件
# Centos执行 yum install curl wget screen -y
# Ubuntu执行 apt-get update -y && apt install curl wget screen -y

# 下述脚本均需要在使用安装脚本时相同的路径执行
# 一键安装GoMinerProxy
bash <(curl -s -L https://raw.githubusercontent.com/GoMinerProxy/GoMinerProxy/main/scripts/install.sh)
# 一键卸载GoMinerProxy
bash <(curl -s -L https://raw.githubusercontent.com/GoMinerProxy/GoMinerProxy/main/scripts/uninstall.sh)
# 一键更新GoMinerProxy到最新版本，可以不关闭GoMinerProxy闪断更新
bash <(curl -s -L https://raw.githubusercontent.com/GoMinerProxy/GoMinerProxy/main/scripts/update.sh)
# 服务器重启后打开 GoMinerProxy
bash <(curl -s -L https://raw.githubusercontent.com/GoMinerProxy/GoMinerProxy/main/scripts/start.sh)
# 重启 GoMinerProxy
bash <(curl -s -L https://raw.githubusercontent.com/GoMinerProxy/GoMinerProxy/main/scripts/restart.sh)
```

```shell
# 再次SSH链接可以使用下述指令查看输出
screen -r go_miner_proxy
```
以上為最簡單的部署示例，您可以參考 [文檔 - 快速開始](https://gominerproxy.github.io/zh_hk/) 進行更為完善的部署。 

## :alembic: 技术栈

* [Go](https://golang.org/) + [Gin](https://github.com/gin-gonic/gin)
* [NodeJs](https://nodejs.org/)
