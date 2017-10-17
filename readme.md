	| 表名              | 表                     | 数据库表说明 | 备注 |
    |:---------------- |:------------------------------- |:--------------------------- |:---------------------|
    | 渠道表            | ULTAB_A_MERCHANT      | IS_CHANNEL ='1'  |  ----ULTAB_BO_CHANNELINFO |
    | 渠道扩展表         | ULTAB_A_MERCEXTENDINFO  |             |             |
    | 渠道配置信息表     | ULTAB_SHP_SERVICE_CONFIG |             |            |
	|  |  |  |
    | 产品提供方表         | ULTAB_A_MERCHANT | IS_ISSUE ='1' |
    | 产品提供方扩展表     | ULTAB_A_MERCEXTENDINFO | |  |
    | 产品提供方配置信息表  | ULTAB_BO_EXT_CODE_MERC | |  |
    |  |  |  |
    | 产品表     		    | ULTAB_BO_VOUCHERPRODINFO |   |
    | 渠道产品表路由        | ULTAB_BO_CHANNEL_PROD |       |
    | 商户产品表路由        | ULTAB_BO_VOUCHERPROD_EXT | |
    |  |  |  |
    | 渠道订单表 | ULTAB_FO_ORDERINFO |   |   |
    | 渠道订单详情表 | ULTAB_FO_ORDERDETAIL |   |   |
    |  |  |  |
    | 订单表 | ULTAB_BO_ORDERINFO(新建) |	  参考ULTAB_BO_ORDERINFO_ZYB |
    | 订单详情 | ULTAB_BO_ORDERDETAIL(新建) |   参考ULTAB_BO_ORDERDETAIL_ZYB |
    |  |  |  |
    | 单张券信息 | ULTAB_BO_VOUCHERINFO |   |   |
    | 单张券信息详细信息 | ULTAB_BO_VOUCHERINFO_EXT |   |   |
