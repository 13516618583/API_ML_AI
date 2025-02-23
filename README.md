# API_ML_AI 
| 发布日期 | 2019.12.2    |
| -------- | ------------ |
| 产品名称 | 智能出行 |
| 文档状态 | 已经完成       |
| 文件主人 | 丘安锋       |
| 设计者   | 丘安锋       |
| 开发者   | 丘安锋       |
| 测试者   | 丘安锋       |
#### 价值主张写作
一句话版本：
- 为解决用户出行安全和企业方便简单管理所做的出行app。

一分钟版本：
- 我们团队做的项目是智能出行app，目前出租车司机的反监控行为（如遮盖车辆摄像头等）、拒载逃单行为（不打表载客、拒绝载客）、从业资格人员非法营运、司机违规违章驾驶行为，这些行为不利于出租车企对于司机行驶营运的管理，理应受到管理部门及企业的处罚。所以我们团队运用百度api中的人脸识别技术、驾驶行为分析技术、语音识别及合成技术的基础上完成一款智能出行app。司机可以在智体出行司机端APP，按照提示完成人脸信息注册；司机在智体出行司机端APP，按照提示完成人脸信息注册；司机上路运营前，车载终端自动调用车载摄像头进行离线人脸识别，确认司机身份进行无感打卡；当核实司机与出租车不存在人车绑定关系时会判定司机打卡不成功，将通过语音合成技术车载智能终端控制多媒体模块播放警告话术。同时，非编”信息同步至出租车企业管理平台及智体出行管理端APP，出租车企业管理平台及APP接收“非编”信息后立即弹出警报消息提醒值班人员并同步记录“非编”日志。
# PATR A 价值主张设计
#### 价值宣言
1、智能出行app通过应用百度大脑人脸识别技术、驾驶行为分析技术、语音识别及合成等多项AI能力，可在行程无感的情况下智能甄别司机信息。 

2、建立反拒载、反逃单、违规驾驶行为报警机制，通过智能终端语音提醒当班司机，以整体提高出租车行业服务质量与形象，让市民出行更加放心。 

3、在人脸识别、驾驶行为分析、语音识别使用过程中，还会结合人工智能算法与容错机制，使得整体误报率低于0.1%。实现了让车内异常情况及报警信息更加精确的送达给企业管理人员，极大减轻企业运维工作成本的同时还提高了企业管理水平，为出租车行业带来技术革新。
#### 核心价值
解决了企业监管难、监管效率低、监管不及时等难点痛点，降低监管成本的同时提升了监管效率，实现了企业管理信息化和智能化。

#### 背景
针对出租车、客车、公交车、货车等各类营运车辆，实时监控车内情况，识别驾驶员抽烟、使用手机、未系安全带等危险行为，及时预警，降低事故发生率，保障人身财产安全 
#### 目标
1. 司机在APP，按照提示完成人脸信息注册，进行实名认证
2. 监测到司机是否存在拒载行为
3. 检测司机是否存在使用手机、抽烟、不系安全带、双手离开方向盘、视角未朝前方等违规驾驶行为

#### 用户
1.出租车企业
2.公交车企业
3.汽车站公司

#### 核心价值与用户痛点
目前出租车司机的反监控行为（如遮盖车辆摄像头等）、拒载逃单行为（不打表载客、拒绝载客）、从业资格人员非法营运、司机违规违章驾驶行为，这些行为不利于出租车企对于司机行驶营运的管理
但目前能够协助出租车企业监管出租车司机驾驶行为的手段及方式少之又少，造成了交通运输管理部门及出租车企的监管困境。 

#### 人工智能概率性
- 智能语音交互准确率在95%以上。百度云智能语音交互用国内独创的字级LC-BLSTM/DFSMN-CTC建模，相对业界传统CTC方法降低了20%的错误率，大幅提高了语音识别的精度。
- 人脸识别准确率达99%。百度云利用上万亿的人脸样本训练模型，识别准确率高。
- 录音太模糊，导致识别的准确率低
- 图片模糊、手机像素过低，导致识别的准确率低

#### 用户需求:（使用的人工智能要反映到需求列表中）

| 用户案例                                   | 对应功能            | 重要程度 |
| ------------------------------------------ | ------------------- | -------- |
| 企业管理员在智行出租车企业管理平台绑定司机与车辆关系；  | 人脸识别| 重要     |
|         司机逃单行为识别，通过车载智能终端媒体播放警告           |     驾驶行为分析技术，语音合成        | 一般     |
| 司机遮盖车辆摄像头 | 反监控行为识别            | 一般     |

#### API的运用
人脸识别，驾驶行为分析，语音合成
# PART B 原型

#### 产品结构图
![Image](https://github.com/13516618583/picture/blob/master/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20191225174700.png)
![Image](https://github.com/13516618583/picture/blob/master/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20200110024753.png)
![Image](https://github.com/13516618583/picture/blob/master/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20200110024759.png)

#### 原型1.交互及界面设计
![Image](https://github.com/13516618583/picture/blob/master/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20191225174731.png)
![Image](https://github.com/13516618583/picture/blob/master/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20191225174913.png)
#### 原型2.信息设计
![Image](https://github.com/13516618583/picture/blob/master/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20191225174929.png)
![Image](https://github.com/13516618583/picture/blob/master/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20191225180106.png)
![Image](https://github.com/13516618583/picture/blob/master/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20200110024809.png)
![Image](https://github.com/13516618583/picture/blob/master/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20200110024804.png)

#### 原型3.原型文档
- [产品原型下载](https://github.com/13516618583/final)

- [产品原型展示](http://qiuanfeng.gitee.io/final ) 

#### 原型4.口头操作说明
司机在智能出行司机端APP，按照提示完成人脸信息注册，企业管理员在智行出租车企业管理平台绑定司机与车辆关系，司机上路运营前，车载终端自动调用车载摄像头进行离线人脸识别，确认司机身份进行无感打卡。
# PART C API
## API使用水平
- API:百度AI--行为分析--驾驶行为分析
- 输入：
 ```
""" 读取图片 """
def get_file_content(filePath):
    with open(filePath, 'rb') as fp:
        return fp.read()

image = get_file_content('example.jpg')

""" 调用驾驶行为分析 """
client.driverBehavior(image);

""" 如果有可选参数 """
options = {}
options["type"] = "smoke"

""" 带参数调用驾驶行为分析 """
client.driverBehavior(image, options)


 ```
 - 输出：
  ```
  {
  "person_num": 1,
  "person_info": [{
    "attributes": {
      "cellphone": {
        "threshold": 0.9,
        "score": 0.500098466873178
      },
      "both_hands_leaving_wheel": {
        "threshold": 0.9,
        "score": 0.468360424041749
      },
      "not_facing_front": {
        "threshold": 0.9,
        "score": 0.08260071277818408
      },
      "not_buckling_up": {
        "threshold": 0.9,
        "score": 0.998087468763092
      },
      "smoke": {
        "threshold": 0.9,
        "score": 6.29425049828125e-05
      }
    },
    "location": {
      "width": 483,
      "top": 5,
      "height": 238,
      "left": 8
    }
  }],
  "log_id": 2320165720061799578
}
 ```
- 百度AI-人脸识别
输入：
 ```
# encoding:utf-8
 import requests

 '''
 人脸检测与属性分析
 '''

import urllib.request,sys,base64
import urllib.parse
request_url = "https://aip.baidubce.com/rest/2.0/face/v3/detect"

f = open('q3.jpg', 'rb')
image = base64.b64encode(f.read())
image64 = str(image,'utf-8')
image_type = "BASE64"




params = {'image': image64,'image_type':"BASE64",'face_field': 'faceshape,facetype'}

params = urllib.parse.urlencode(params).encode("utf-8")


access_token = '[24.b5ff1af7ad57860f4a47b0972dd0560f.2592000.1579764577.282335-18098227]'
request_url = request_url + "?access_token=" + access_token

request = urllib.request.urlopen(url=request_url, data=params)   

content = request.read()  
print(content) 

 ```
 
 输出：
 ```
 (b'{"error_code":0,"error_msg":"SUCCESS","log_id":19955551594,"timestamp":15771'
 b'72758,"cached":0,"result":{"face_num":1,"face_list":[{"face_token":"3d44d56f'
 b'3d2d41190368b2697023d5f2","location":{"left":235.97,"top":819.91,"width":426'
 b',"height":446,"rotation":0},"face_probability":0.95,"angle":{"yaw":-7.9,"pit'
 b'ch":-5.58,"roll":-4.76},"face_shape":{"type":"square","probability":0.52},"f'
 b'ace_type":{"type":"human","probability":1}}]}}')

 ```
## API使用比较分析
### 自身分析
##### 百度AI-人脸识别
- 算法世界领先 ：
基于百度专业的深度学习算法和海量数据训练，人脸识别算法在最权威的公开评测比赛中排名世界领先 
- 服务稳定高效 
提供企业级稳定、精确的大流量服务。支持毫秒级的识别响应能力、弹性灵活的高并发 
- 灵活简单易用 ：
可自定义接口的返回参数信息，灵活组合各项人脸技术模块，实现不同业务功能 
##### 百度AI-驾驶行为识别
- 深入场景 ：
专项训练高精度识别模型，覆盖出租车、客车、公交车、货车等典型车载场景 
- 应用灵活 
针对每类属性行为，分别返回概率分数和建议阈值，可根据实际业务需求灵活设置 
- 服务稳定 
可提供企业级稳定、精确的大流量服务，拥有毫秒级识别响应能力及99.9%的可靠性保障 

### 竞争对手分析
##### 阿里云智能人脸识别
- 识别精度高、解码速率快、反馈时间短， 免费只有试用套餐，收费使用价格较高。

##### 总结
- 百度方和阿里方各有各的产品优势、技术优势，但是百度的API调用性价比较高，所以比较推荐使用百度的API

## API使用后风险报告
- 驾驶行为分析次数包上新开售，高性价比“行车安全保障”，优惠后接口调用低至0.7元/千次。
- 目前API市场上，提供“驾驶行为识别”这一API接口服务的公司还是比较少的，只有百度AI这一家，竞争压力小。
- 目前API市场上，提供“人脸识别”这一API接口服务的公司还是比较多的，百度、阿里、腾讯、微软等等，竞争压力大。
- 百度人脸识别不支持不支持GIF图片。



