<img src="https://archost.com/wp-content/uploads/2022/12/Icon-blue-512x512-1.png" alt="logo" width="130" height="130" align="right"/>

# ** DIY Xray Node **

A backend structure built on Xray that can easily handle a variety of panels and is compatible with V2ray, Trojan, and Shadowsocks protocols. Additionally, it is effortless to extend and can be connected to multiple panels.

## One Click install product
[Setup Now](https://my.archost.com/store/diy-vpn/diy-xray-node)

## Document
[Click](https://my.archost.com/knowledgebase/7011/DIY-Xray-Node)

## Linux Installation

```
bash <(curl -Ls https://raw.githubusercontent.com/XrayR-project/XrayR-release/master/install.sh)
```
## Docker installation

```
docker pull ghcr.io/xrayr-project/xrayr:latest && docker run --restart=always --name xrayr -d -v ${PATH_TO_CONFIG}/config.yml:/etc/XrayR/config.yml --network=host ghcr.io/xrayr-project/xrayr:latest
```

## Docker compose
0. Install docker-compose: 
```
curl -fsSL https://get.docker.com | bash -s docker
curl -L "https://github.com/docker/compose/releases/download/1.26.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```
1. `git clone https://github.com/XrayR-project/XrayR-release`
2. `cd XrayR-release`
3. Edit config. The basic format of the configuration file is as follows. Multiple panels and multiple node configuration information can be added under Nodes at the same time, just add the Nodes item in the same format.
4. Start docker:docker-compose up -d`

## Docker compose upgrade

Execute in the docker-compose.yml directory:

```
docker-compose pull
docker-compose up -d
```

## Community
🔔Telegram Channel: [@archostofficial](https://t.me/archostofficial)  

## How to Feedback
Follow the template in the issue to submit your question correctly, and we will have someone follow up with you.
