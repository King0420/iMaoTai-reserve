
# i茅台预约工具----宝塔版

<p align="center">
  <a href="https://hits.seeyoufarm.com">
     <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FKing0420%2FiMaoTai-reserve&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/>
  </a>
  <a href="https://github.com/King0420/iMaoTai-reserve">
    <img src="https://img.shields.io/github/stars/King0420/iMaoTai-reserve" alt="GitHub Stars">
  </a>
  <a href="https://github.com/King0420/iMaoTai-reserve">
    <img src="https://img.shields.io/github/forks/King0420/iMaoTai-reserve" alt="GitHub Forks">
  </a>
  <a href="https://github.com/King0420/iMaoTai-reserve/issues">
    <img src="https://img.shields.io/github/issues-closed-raw/King0420/iMaoTai-reserve" alt="GitHub Closed Issues">
  </a>
  <a href="https://github.com/King0420/iMaoTai-reserve">
    <img alt="GitHub commit activity (branch)" src="https://img.shields.io/github/commit-activity/y/King0420/iMaoTai-reserve">
  </a>
  <a href="https://github.com/King0420/iMaoTai-reserve">
    <img src="https://img.shields.io/github/last-commit/King0420/iMaoTai-reserve" alt="GitHub Last Commit">
  </a>
</p>


### 功能：
- [x] 集成Github Actions
- [x] 多账号配置
- [x] 账号有效期管控
- [x] 手机号加密保存
- [x] 自动获取app版本
- [x] 微信消息推送

### 原理：
```shell
1、登录获取验证码
2、输入验证码获取TOKEN
3、获取当日SESSION ID
4、根据配置文件预约CONFIG文件中，所在城市的i茅台商品
```


### 使用方法：

### 1、安装依赖
```shell
pip3 install --no-cache-dir -r requirements.txt
```
或者
```shell
pip3 install requests
pip3 install pycryptodome==3.17
```

### 2、修改config.py，按照你的需求修改相关配置，这里很重要，建议每个配置项都详细阅读。


### 3、按提示输入 预约位置、手机号、验证码 等，生成的token等。很长时间不再需要登录。支持多账号，支持加密。
1. 第一次使用先清空`./myConfig/credentials`中的信息，或者直接删除`credentials`文件也可以
2. 再去配置环境变量 `GAODE_KEY`,再运行`login.py`.
```shell
python3 login.py
# 都选择完之后可以去./myConfig/credentials中查看
```

### 4、python3 main.py ,执行预约操作
```shell
python3 main.py
```

### 5、配置宝塔面板，每日自动预约。
- 先Fork本项目，再去自己的项目中配置`PUSHPLUS_KEY`和和`PRIVATE_AES_KEY`

#### 欢迎请我喝咖啡（O.o），对我下班和周末时光的努力进行肯定，您的赞赏将会给我带来更多动力。或者动动小手点个小星星

<img src="resources/imgs/wxqr.png" height="300">  <img src="resources/imgs/zfbqr.jpg" height="300">


