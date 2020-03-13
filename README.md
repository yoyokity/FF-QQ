# **FF-QQ使用简单说明**
实现FF文本指令与QQ之间的双向转发   
   
    
	
开发小组：念冬、yoyokity、souma、蒙特拉、Kyouko、千夏


----------

> 准备：    
> 1、酷Q机器人 （和自己QQ是好友）   
> 2、挂机器人的服务器      
> 3、ACT trigger插件    
> 4、Post Namazu  
> 
> 最后，确保你玩游戏的机子在公网或者做了内网穿透


酷Q端使用方法：QQ→FF

 - 安装酷Q插件：CQ_QQ to PostNamazu.cpk
 - 向机器人发送信息：/ip (IP:post) 来设定IP  （确保酷Q的机子能通过该IP和post，连接到本机的post namazu程序）
 - 使用【#+宏指令】向QQBOT发送宏指令，并自动转发到游戏内。例如：【#/fc 部队频道】【#/ac 冲刺】【#/挥手】


ACT端使用方法：FF→QQ

 - 导入trigger：trigger_FF to CQ.xml
 - 进入设置，“獭獭”和“自己配置”2选1
 - 獭獭使用的是獭爹的模块，要设置自己QQ，机器人QQ，token，详见獭爹NGA帖子。缺点是内置5秒CD，会忽略5秒内的信息
 - 自己配置则是字面意思，要你自己配置酷Q的HTTPAPI，需要设置自己QQ，机器人所在主机IP，token。token是httpapi的配置文件中设置的。这个模块则不会像獭獭模块有5秒CD，post默认5700不要去动！
 - 如果你的机器人装了獭獭的API配置，但还是想用“自己配置”模块，很简单 “use_http”项目的值改成“true”，token则是你獭獭的token（你直接看一下“token”项目的值就行）


特殊指令：   
#/e 关机：直接关机

#/e 关闭游戏：关闭FFXIV
