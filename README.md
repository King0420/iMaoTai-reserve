
# i茅台每日申购----宝塔版
> 预约时间：每天9点-10点
> 
> 酒的种类：53%vol 500ml贵州茅台酒（甲辰龙年）和 53%vol 375ml×2贵州茅台酒（甲辰龙年）


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

![iMaoTai-reserve](https://socialify.git.ci/King0420/iMaoTai-reserve/image?description=1&forks=1&language=1&name=1&owner=1&pattern=Plus&stargazers=1&theme=Light)

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

### 2、修改config.py，按照你的需求修改相关配置，分为必须配置选项和可选配置选项。
#### 必须配置选项
**地图配置**：[申请KEY教程](https://lbs.amap.com/api/webservice/create-project-and-key)

![image](https://github.com/King0420/iMaoTai-reserve/assets/104044278/4bbf1834-1d9d-40a6-bf9d-26674cc6c418)

**个人加解密密钥配置**：
![image](https://github.com/King0420/iMaoTai-reserve/assets/104044278/fc6fa8da-14c2-4daa-a1c0-7fc8eb7b89b5)

#### 可选配置选项
**消息推送配置**：
![image](https://github.com/King0420/iMaoTai-reserve/assets/104044278/835123f4-37aa-473e-b794-545f08811c24)


### 3、按提示输入 预约位置、手机号、验证码 等，生成的token等。很长时间不再需要登录。支持多账号，支持加密。
1. 先删除myConfig文件夹下的`credentials`文件.
2. 然后再运行`login.py`.
3. 运行完login.py可以去./myConfig/credentials中查看.
```shell
python3 login.py
```
**运行结果示例**
```shell
mobian@mobian:~/app/imaotai$ python3 login.py

请输入你的位置,例如[小区名称],为你预约本市门店商店: 军安家园
0 : [地区:内蒙古自治区,位置:内蒙古自治区赤峰市红山区军安家园]
请选择位置序号,重新输入请输入[-]:0
已选择 地区:北京市,[北京市海淀区上地十街]附近的门店
输入手机号[13812341234]:1861164****
输入 [1861164****] 验证码[1234]:1234
是否继续添加账号[Y/N]:n
```

### 4、python3 main.py ,执行预约操作
```shell
python3 main.py
```
![image](https://github.com/King0420/iMaoTai-reserve/assets/104044278/cd04ba52-70b1-4080-b766-116eadc87890)

### 5、配置宝塔面板，每日自动预约。
![image](https://github.com/King0420/iMaoTai-reserve/assets/104044278/2c88f9d5-5e44-43ab-b3df-b5240a74c3b6)




### Star History

[![Star History Chart](https://api.star-history.com/svg?repos=King0420/iMaoTai-reserve&type=Date)](https://star-history.com/#King0420/iMaoTai-reserve&Date)



### 推荐
- [i茅台app使用windows服务器每日自动预约](https://github.com/lisongkun/HyggeImaotai)
- [wd210010/only_for_happly: 农夫山泉龙年抽水签到任务★恩山签到★雨云签到白嫖服务器★小茅预约★丽宝乐园小程序签到★天翼云盘签到★腾讯视频签到（会员领成长值）★阿里云盘签到★GW树洞机场签到★富贵论坛签到★一点万向签到打卡★什么值得买达人和关键词取消关注★STLXZ签到★PT站签到★帆软签到+摇摇乐★千图网签到★星空代理签到★什么值得买签到★值得买每日抽奖★小米社区签到★逑美在线app签到和抽卡★ddnsto自动续费七天★爱奇艺签到刷时长★双色球预测（娱乐） (github.com)](https://github.com/wd210010/only_for_happly)
- [i茅台，葫芦娃预约脚本](https://github.com/yize8888/maotai)

### 帮忙点个小星星。

| 53%vol 500ml贵州茅台酒（甲辰龙年）                           | 53%vol 375ml×2贵州茅台酒（甲辰龙年）                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![](https://github.com/King0420/iMaoTai-reserve/assets/104044278/9459c994-cd84-4ac6-884b-ba0c4c63c2c1) | ![](https://github.com/King0420/iMaoTai-reserve/assets/104044278/17acd549-85be-431b-b0f9-a8148c1ce87f) |

