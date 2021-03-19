# Ubuntu Installation
1. 制作启动盘
2. 设置u盘启动
3. 安装系统


## 常用设置
1. 系统设置
2. tweak 安装, tweak 设置
3. 键位设置


## 别名设置
```bash
apt install vim-gtk3  #gtk3 支持剪切板

# 设置别名  vim .bash_profile
alias apt-get="sudo apt-get"
alias apt="sudo apt"
alias systemctl="sudo systemctl"
alias netstat="sudo netstat"
alias snap="sudo snap"

source .bash_profile #使配置生效
```

## apt 加速
```bash
sudo cp /etc/apt/source.list /etc/apt/source.list.back
sudo vim etc/apt/source.list

deb http://mirrors.aliyun.com/ubuntu/ bionic main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ bionic-security main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ bionic-updates main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ bionic-proposed main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ bionic-backports main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ bionic main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ bionic-security main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ bionic-updates main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ bionic-proposed main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ bionic-backports main restricted universe multiverse

# update apt
apt update
```

