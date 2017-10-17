#优方产品平台项目

####一、角色
>1.优方产品平台
		
		说明   ：将产品提供方的产品维护到产品库中
		        将供货方交易接口调用配置参数保存到表中
		
		产品分类：
		        电子券:如宜芝多电子券
		        购物卡：如DQ充值卡
		        流量话费：99无限话费充值
		        
		
>2.渠道：

		渠道指的是销售平台
		如天猫商城、江苏移动商城、工商商城、微信商城等
		
>3.产品提供方：

		优方供货方
		外部供货方，如银商资讯、99无限等
		
####二.流程(以优方产品平台为中心)
 
    1.将产品提供方的产品维护到产品库中
	2.将渠道产品编号关联到产品库中产品
	3.对渠道提供交易接口调用及进行对账
	4.调用产品提供方交易接口及进行对账
	
	       调用	                      调用
    	渠道-----------> 优方产品平台 ---------> 产品提供方接口

####三、相关表
    
    <table>
        <tr>
            <th>表名</th><th>表</th><th>数据库表说明</th><th>备注 </th>
        </tr>
        <tr>
            <td>渠道表</td><td>ULTAB_A_MERCHANT|ULTAB_BO_CHANNELINFO</td><td></td><td>IS_CHANNEL ='1'</td>
        </tr>
        <tr>
            <td>渠道扩展表</td><td>ULTAB_A_MERCEXTENDINFO</td><td></td><td></td>
        </tr>
        <tr>
            <td>渠道配置信息表</td><td>ULTAB_SHP_SERVICE_CONFIG</td><td></td><td></td>
        </tr>
        <tr>
            <td></td><td></td><td></td><td></td>
        </tr>
        <tr>
            <td>产品提供方表</td><td>ULTAB_A_MERCHANT </td><td></td><td>IS_ISSUE ='1'</td>
        </tr>
        <tr>
            <td>产品提供方扩展表</td><td>ULTAB_A_MERCEXTENDINFO</td><td></td><td></td>
        </tr>
        <tr>
            <td>产品提供方配置信息表</td><td>ULTAB_BO_EXT_CODE_MERC</td><td></td><td></td>
        </tr>
        <tr>
            <td></td><td></td><td></td><td></td>
        </tr>
        <tr>
            <td>产品表</td><td>ULTAB_BO_VOUCHERPRODINFO</td><td></td><td></td>
        </tr>
        <tr>
            <td>渠道产品表路由</td><td>ULTAB_BO_CHANNEL_PROD</td><td></td><td></td>
        </tr>
        <tr>
            <td>商户产品表路由</td><td>ULTAB_BO_VOUCHERPROD_EXT</td><td></td><td></td>
        </tr>
        <tr>
            <td></td><td></td><td></td><td></td>
        </tr>
        <tr>
            <td>渠道订单表</td><td>ULTAB_FO_ORDERINFO</td><td></td><td></td>
        </tr>
        <tr>
            <td>渠道订单详情表</td><td>ULTAB_FO_ORDERDETAIL</td><td></td><td></td>
        </tr>
        <tr>
            <td>订单表</td><td>ULTAB_BO_ORDERINFO(新建)</td><td></td><td></td>
        </tr>
        <tr>
            <td>订单详情</td><td>ULTAB_BO_ORDERDETAIL(新建)</td><td></td><td></td>
        </tr>
         <tr>
            <td>单张券信息</td><td>ULTAB_BO_VOUCHERINFO</td><td></td><td></td>
        </tr>
        <tr>
            <td>单张券信息详细信息</td><td>ULTAB_BO_VOUCHERINFO_EXT</td><td></td><td></td>
        </tr>
    </table>
   
   
   | 表头1  | 表头2|
   | ---------- | -----------|
   | 表格单元   | 表格单元   |
   | 表格单元   | 表格单元   |
   
   ### 对齐
   表格可以指定对齐方式
   
   | 左对齐 | 居中  | 右对齐 |
   | :------------ |:---------------:| -----:|
   | col 3 is      | some wordy text | $1600 |
   | col 2 is      | centered        |   $12 |
   | zebra stripes | are neat        |    $1 |
   
   
#### 四、项目结构
   
    product-commons: 通用部分
    product-dao: 数据库操作层
    product-marchant-serivce:调用产品提供方服务
    product-service:渠道方调用 优方产品平台服务
    product-controller:对外提供访问的路由
    
#### 五、实现步骤（待开发）
    
