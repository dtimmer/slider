# slider
一个多滑块插件，需要slider.init(document.getElementById('...'))进行初始化，然后通过返回的对象进行setOption生成
目前需要提前加载jquery，后续会逐渐去掉jquery的依赖
配置option:
 * option基础模型(该模型初始值都为0)
 * type:类型，normal为普通滑块类型，block为分块滑块，默认值为normal
 * class:根据num来进行分级，如果num出现一致，则初始化失败,每个区块有单独的颜色配置，最大值为上限，不设置max,min的原因在于每个区间可以自定义颜色
 * 默认两个滑块不能重叠和超出，距离至少为1
 * option = {
 * 		type: 'normal/block',
 * 		class: [
 * 			{
 * 				color: #fff,
 * 				num: 10
 * 			},...
 * 		]
 * }
 * 
![image](https://github.com/dtimmer/slider/edit/master/cc.png)
