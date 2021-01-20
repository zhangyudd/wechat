### 链接跳转微信小程序

[h5jump_wechat.html](https://github.com/zhangyudd/wechat/blob/master/h5jump_wechat.html)

* 替换静态页面中，注释为replace的行

* 小程序schmma获取方式

  * 获取access_token:

  `https://api.weixin.qq.com/cgi-bin/token?grant_type=client_credential&appid=appid&secret=secret`

  * 获取小程序schmma:

    `POST请求`

    `https://api.weixin.qq.com/wxa/generatescheme?access_token=access_token`

    `Headers:	Content-Type:application/json`

    `Body:    raw   `

    `{
        "jump_wxa":
        {
            "path": "/pages/index/index",
            "query": ""
    	    },
        "is_expire":false
    }`

    

    



