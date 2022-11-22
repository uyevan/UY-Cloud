### <font class="text-color-6" color="#2196f3">💛💻⌨UY云用户开放API接🚥🧺🌬</font>

----

* <font class="text-color-2" color="#e91e63">用户注册</font>：uyapi/uyyun_userreg.php
提交方式：必POST
```
提交参数：
keeper（后台账号）
api（应用api）
user（注册账号）
pass（注册密码）
qq（用户QQ）
name（用户名称）
file（用户头像，是提交头像文件）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：注册成功/注册失败）
```
> 请求实例：http://yun.jfkj.xyz/uyapi/uyyun_register.php?keeper=后台账号&api=应用API&user=xxx&pass=xxx&qq=xxx&name=xxx&file=头像File文件

 
----


* <font class="text-color-2" color="#e91e63">用户登录</font>：uyapi/uyyun_login.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（登录账号）
pass（登录密码）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：登录成功/登录失败）
name（用户名称）
 QQ（用户qq）
signtext（用户签名-暂时不可改）
regtime（注册时间）
vip（是否会员true/false）
seal（账号是否封禁）
viptime（会员时间）
userhead（用户头像）
UYcoin（UY币）
```

> 请求实例：http://yun.jfkj.xyz/uyapi/uyyun_login.php?keeper=后台账号&api=应用API&user=xxx&pass=xxx

 
----

* <font class="text-color-2" color="#e91e63">判断用户会员</font>：uyapi/uyyun_uservip.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：是会员用户/不是会员用户）
ifvip（是否会员 true/false）
```

>请求实例：http://yun.jfkj.xyz/uyapi/uyyun_uservip.php?keeper=后台账号&api=应用API&user=xxx&pass=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户签到</font>：uyapi/uyyun_user_sign.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：已签到/签到失败）
```

>请求实例：http://yun.jfkj.xyz/uyapi/uyyun_user_sign.php?keeper=后台账号&api=应用API&user=xxx&pass=xxx
提示：会员用户和普通用户签到得到的金币数量可自定义，账号封禁或其他情况无法签到。

----

* <font class="text-color-2" color="#e91e63">用户信息数据获取</font>（私有）：uyapi/uyyun_userdate.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（登录账号）
pass（登录密码）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
name（用户名称）
QQ（用户qq）
signtext（用户签名）
regtime（注册时间）
vip（是否会员true/false）
viptime（会员时间）
seal（账号是否封禁）
userhead（用户头像）
UYcoin（UY币）
```

>请求实例：http://yun.jfkj.xyz/uyapi/uyyun_userdate.php?keeper=后台账号&api=应用API&user=xxx&pass=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户信息数据获取</font>（公有）：uyapi/user_date.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（登录账号）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
name（用户名称）
QQ（用户qq）
signtext（用户签名）
regtime（注册时间）
vip（是否会员true/false）
viptime（会员时间）
seal（账号是否封禁）
userhead（用户头像）
UYcoin（UY币）
```

>请求实例：http://yun.jfkj.xyz/uyapi/user_date.php?keeper=后台账号&api=应用API&user=xxx

----

* <font class="text-color-2" color="#e91e63">应用更新</font>：uyapi/preview_newapp.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：获取成功/获取失败）
 newappedition（应用版本）
 newappcontent（更新内容）
 newappdowurl（新版下载地址）
 newappimgurl（更新一张图片）
 newappstyle（是否为强制更新true/false）
```

>请求实例：http://yun.jfkj.xyz/uyapi/preview_newapp.php?keeper=后台账号&api=应用API
提示：新版下载地址可直链也可别的，更多的你可以在前端自由实现
 
----

* <font class="text-color-2" color="#e91e63">应用公告</font>：uyapi/preview_notice.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：获取成功/获取失败）
notice（公告内容）
noticetype（公告类型或分类）
```

>请求实例：http://yun.jfkj.xyz/uyapi/preview_notice.php?keeper=后台账号&api=应用api
 
----

* <font class="text-color-2" color="#e91e63">应用通知列表</font>：uyapi/ukturux_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
id（通知ID）
title（通知标题）
content（通知内容）
imgurl（图片地址）
sendtime（通知发布时间）
```

>请求实例：http://yun.jfkj.xyz/uyapi/ukturux_list.php?keeper=后台账号&api=应用api
 
----

* <font class="text-color-2" color="#e91e63">文档查看</font>：uyapi/file_preview.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
title（文档名）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
id（文档ID）
title（文档名）
content（文档内容）
type（文档类型）
url（当文件是HTML模式的URL链接）
```

>请求实例：http://yun.jfkj.xyz/uyapi/file_preview.php?keeper=后台账号&api=应用API&title=文档名
提示：本API只用来查看文档数据（全数据）
 
----

* <font class="text-color-2" color="#e91e63">TEXT文档查看</font>：uyapi/file_text.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
title（文档名）
返回数据：
直接返回TEXT文档内容
```

>请求实例：http://yun.jfkj.xyz/uyapi/file_text.php?keeper=后台账号&api=应用API&title=文档名
提示：本API只用来查看TETX文档内容的，会直接返回文档内容，无其他参数
 
----

* <font class="text-color-2" color="#e91e63">商品列表</font>：uyapi/pay_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
id（商品ID）
title（商品名）
intro（商品介绍）
frice（商品价格，全平台统一用UY币）
sendtime（商品添加时间）
num（商品库存数量）
type（商品类型，VIP购买商品或TEXT商品）
lose（会员用户打折率 ，0至1）
icon（商品图片链接）
```

>请求实例：http://yun.jfkj.xyz/uyapi/pay_list.php?keeper=后台账号&api=应用API
 
----

* <font class="text-color-2" color="#e91e63">商品搜索列表</font>：uyapi/pay_search.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
title（商品标题或商品名）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
id（商品ID）
title（商品名）
intro（商品介绍）
frice（商品价格，全平台统一用UY币）
sendtime（商品添加时间）
num（商品库存数量）
type（商品类型，VIP购买商品或TEXT商品）
lose（会员用户打折率 ，0至1）
icon（商品图片链接）
```

>请求实例：http://yun.jfkj.xyz/uyapi/pay_search.php?keeper=后台账号&api=应用API&title=商品名
 
----

* <font class="text-color-2" color="#e91e63">商品购买</font>：uyapi/pay_userbay.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
id（购买商品的ID）
email（如果是TEXT商品则必须提交，会员商品可不提交）
返回数据：
如果是VIP会员商品返回：
code：true（成功）/false（失败）
 msg=返回请求结果（会员开通至到期时间）如果是TEXT文本商品：
code：true（成功）/false（失败）
 msg=返回请求结果（会把TEXT商品的内容发到提交的邮箱）
```

>会员商品请求实例：http://yun.jfkj.xyz/uyapi/pay_userbay.php?keeper=后台账号&api=应用API&user=购买用户账号&pass=购买用户密码&id=商品ID
TEXT商品请求实例：http://yun.jfkj.xyz/uyapi/pay_userbay.php?keeper=后台账号&api=应用API&user=购买用户账号&pass=购买用户密码&id=商品ID&email=xxx@qq.com
 
----


* <font class="text-color-2" color="#e91e63">商品搜索查看</font>：uyapi/pay_preview.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
id（商品ID）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
id（商品ID）
title（商品名）
intro（商品介绍）
frice（商品价格，全平台统一用UY币）
sendtime（商品添加时间）
num（商品库存数量）
type（商品类型，VIP购买商品或TEXT商品）
lose（会员用户打折率 ，0至1）
icon（商品图片链接）
```

>请求实例：http://yun.jfkj.xyz/uyapi/pay_preview.php?keeper=后台账号&api=应用API&id=商品ID
 
----

* <font class="text-color-2" color="#e91e63">应用商店列表</font>：uyapi/appstore_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
vipapp（是否只输出会员应用, 如=vipapp则输出会员应用，空则所有应用，可空）
outtype（应用列表输出方式，asc--正序，不填或空则倒序，可空）
返回数据：
code：true（成功）/false（失败）
id（应用ID）
 icon（应用图标链接）
 name（应用名）
 content（应用介绍）
 size（大小）
 edition（应用版本）
 img1（应用截图1）
 img2（应用截图2）
 img3（应用截图3）
 auther（应用作者）
 ifvip（是否是会员应用）
 sendtime（应用发布时间）
 sort（应用分类）
```

>请求实例：http://yun.jfkj.xyz/uyapi/appstore_list.php?keeper=后台账号&api=应用API&outtype=asc(只能填asc别的不行)&vipapp=vipapp(只能填vipapp填别的输出所有应用)
 
----

* <font class="text-color-2" color="#e91e63">应用商店按分类列表</font>：uyapi/appstore_sort_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
sort（应用分类名，如：工具箱/Tools）
vipapp（是否只输出会员应用, 如=vipapp则输出会员应用，空则所有应用，可空）
outtype（应用列表输出方式，asc--正序，不填或空则倒序，可空）
返回数据：
code：true（成功）/false（失败）
 id=返回请求结果（如：成功/失败）
id（应用ID）
 icon（应用图标链接）
 name（应用名）
 content（应用介绍）
 size（大小）
 edition（应用版本）
 img1（应用截图1）
 img2（应用截图2）
 img3（应用截图3）
 auther（应用作者）
 ifvip（是否是会员应用）
 sendtime（应用发布时间）
 sort（应用分类）
```

>请求实例：http://yun.jfkj.xyz/uyapi/appstore_sort_list.php?keeper=后台账号&api=应用API&sort=应用分类名&outtype=asc(只能填asc别的不行)&vipapp=vipapp(只能填vipapp填别的输出所有应用)
 
----

* <font class="text-color-2" color="#e91e63">应用商店搜索列表</font>：uyapi/appstore_search.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
name（应用名）
返回数据：
code：true（成功）/false（失败）
 id=返回请求结果（如：成功/失败）
id（应用ID）
 icon（应用图标链接）
 name（应用名）
 content（应用介绍）
 size（大小）
 edition（应用版本）
 img1（应用截图1）
 img2（应用截图2）
 img3（应用截图3）
 auther（应用作者）
 ifvip（是否是会员应用）
 sendtime（应用发布时间）
 sort（应用分类）
```

>请求实例：http://yun.jfkj.xyz/uyapi/appstore_search.php?keeper=后台账号&api=应用API&name=应用名
 
----

* <font class="text-color-2" color="#e91e63">应用商店按作者列表</font>：uyapi/appstore_auther_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
auther（应用作者名，如：Evan/八特）
vipapp（是否只输出会员应用, 如=vipapp则输出会员应用，空则所有应用，可空）
outtype（应用列表输出方式，asc--正序，不填或空则倒序，可空）
返回数据：
code：true（成功）/false（失败）
 id=返回请求结果（如：成功/失败）
id（应用ID）
 icon（应用图标链接）
 name（应用名）
 content（应用介绍）
 size（大小）
 edition（应用版本）
 img1（应用截图1）
 img2（应用截图2）
 img3（应用截图3）
 auther（应用作者）
 ifvip（是否是会员应用）
 sendtime（应用发布时间）
 sort（应用分类）
```

>请求实例：http://yun.jfkj.xyz/uyapi/appstore_auther_list.php?keeper=后台账号&api=应用API&auther=应用作者名&outtype=asc(只能填asc别的不行)&vipapp=vipapp(只能填vipapp填别的输出所有应用)
 
----

* <font class="text-color-2" color="#e91e63">应用详细</font>：uyapi/appstore_preview.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user(用户账号)
pass(用户密码)
id（应用ID）
返回数据：
code：true（成功）/false（失败）
 id=返回请求结果（如：成功/失败）
id（应用ID）
 icon（应用图标链接）
 name（应用名）
 content（应用介绍）
 size（大小）
 edition（应用版本）
 img1（应用截图1）
 img2（应用截图2）
 img3（应用截图3）
 auther（应用作者）
 dowurl（下载地址,会员应用则判断再返回数据）
 sendtime（应用发布时间）
 sort（应用分类）
```

>请求实例：http://yun.jfkj.xyz/uyapi/appstore_preview.php?keeper=后台账号&api=应用API&user=xxx&pass=xxx&id=应用ID
提示：如果不是会员，但预览会员应用是可以正常预览，但是下载地址返回：“你不是会员用户”。
 
----

* <font class="text-color-2" color="#e91e63">影视列表</font>：uyapi/vedio_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
id（应用ID）
 img（电影封面链接）
 name（电影名）
 content（电影介绍）
 auther（自定义参数，你可以理解为电影分类来使用~）
 ifvip（是否会员类电影）
 ifuycoin（是否是UY购买类型电影）
 uycoinnum（如UY币购买类型，则UY币数量）
 ifmore（是否多集影视）
```

>请求实例：http://yun.jfkj.xyz/uyapi/vedio_list.php?keeper=后台账号&api=应用API
 
----

* <font class="text-color-2" color="#e91e63">影视按自定义参数列表</font>：uyapi/vedio_auther_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
auther（这是auther参数，是个自定义参数。可影视分类也可别的）
返回数据：
 code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
 id（应用ID）
 img（电影封面链接）
 name（电影名）
 content（电影介绍）
 auther（自定义参数，你可以理解为电影分类来使用~）
 ifvip（是否会员类电影）
 ifuycoin（是否是UY购买类型电影）
 uycoinnum（如UY币购买类型，则UY币数量）
 ifmore（是否多集影视）
```

>请求实例：http://yun.jfkj.xyz/uyapi/vedio_auther_list.php?keeper=后台账号&api=应用API&auther=参数auther
 
----

* <font class="text-color-2" color="#e91e63">影视搜索列表</font>：uyapi/vedio_search.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
name（电影名）
返回数据：
 code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
 id（应用ID）
 img（电影封面链接）
 name（电影名）
 content（电影介绍）
 auther（自定义参数，你可以理解为电影分类来使用~）
 ifvip（是否会员类电影）
 ifuycoin（是否是UY购买类型电影）
 uycoinnum（如UY币购买类型，则UY币数量）
 ifmore（是否多集影视）
```

>请求实例：http://yun.jfkj.xyz/uyapi/vedio_search.php?keeper=后台账号&api=应用API&name=电影名
 
----

* <font class="text-color-2" color="#e91e63">影视详细</font>：uyapi/vedio_preview.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
id（影视ID）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：成功/失败）
id（应用ID）
 img（封面链接）
 name（电影名）
 content（电影介绍）
 auther（自定义参数，你可以理解为电影分类来使用~）
 ifvip（是否会员类电影）
 ifuycoin（是否是UY购买类型电影）
 uycoinnum（如UY币购买类型，则UY币数量）
 ifmore（是否多集影视）
```

>请求实例：http://yun.jfkj.xyz/uyapi/vedio_preview.php?keeper=后台账号&api=应用API&id=电影ID
 
----

* <font class="text-color-2" color="#e91e63">影视播放</font>：uyapi/vedio_play.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
id（播放电影的ID）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果（如：成功/失败）
img（电影封面）
name（电影名）
content（电影介绍）
playurl（电影播放地址，播放器请自己适配）
id（电影id）
ifvip（是否会员电影）
ifuycoin（是否UY币电影）
uycoinnum（UY币数量）	
ifmore（是否多集电影）
moredate（多集电影数据）
```

>请求实例：http://yun.jfkj.xyz/uyapi/vedio_play.php?keeper=后台账号&api=应用API&user=播放用户账号&pass=播放用户密码&id=电影ID
提示：用户是会员且UY币可够才会返回以上数据，否则不会返回。
 
----

* <font class="text-color-2" color="#e91e63">应用托管</font>：deposit.php
提交方式：POST/GET

```
提交参数：
appid（应用api）
返回数据：
直接访问
```

>请求实例：http://yun.jfkj.xyz/deposit.php?appid=您的应用API
提示：（API=api=appid=APPid=appID=应用api）且每个应用api平台唯一
 
----

* <font class="text-color-2" color="#e91e63">卡密查询及搜索</font>：uyapi/cdkey_seach.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
type（卡密类型，目前仅有两种会员和UY币类型，搜索值分别为：vip和coin）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（如：存在该类型卡密/不存在该类型卡密）
```

>请求实例：http://yun.jfkj.xyz/uyapi/cdkey_seach.php?keeper=后台账号&api=应用API&type=卡密类型（vip或coin）
 
----

* <font class="text-color-2" color="#e91e63">用户使用卡密</font>：uyapi/cdkey_user_use.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
key（18位卡密）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果（返回会员开通时间值，或UY币充值数量结果）
```

>请求实例：http://yun.jfkj.xyz/uyapi/cdkey_user_use.php?keeper=后台账号&user=用户账号&pass=用户密码&api=应用API&key=18位卡密
 
----

* <font class="text-color-2" color="#e91e63">机器人咨询</font>：uyapi/robot_use.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
come（问题或收到的内容）
返回数据：
如果成功会直接返回后台布置的内容或数据，搜索依据：只要收到的数据存在于后台数据库中，就会返回那个设置的返回数据。
```

>请求实例：http://yun.jfkj.xyz/uyapi/robot_use.php?keeper=后台账号&api=应用API&come=用户发起问题或内容
 
----

* <font class="text-color-2" color="#e91e63">用户支付购买会员</font>：userpay/vip.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
value（会员月数量，只能1/12的整数）
type（支付类型（wxpay/alipay/qqpay）仅三种类型）
返回数据：
code：true（成功）/false（失败）
 msg=返回支付结果
```

>请求实例：http://yun.jfkj.xyz/userpay/vip.php?keeper=后台账号&api=应用API&user=用户账号&value=购买会员月数量&type=支付方式（wxpay/alipay/qqpay）
提示：这个支付请求必须要用网页来请求，你可以软件里写一个浏览器或者跳转浏览器都行。这个不是数据请求，把值填好转到WebView就可以。
 
----

* <font class="text-color-2" color="#e91e63">用户支付购买UY币</font>：userpay/coin.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
value（UY币数量，整数）
type（支付类型（wxpay/alipay/qqpay）仅三种类型）
返回数据：
code：true（成功）/false（失败）
 msg=返回支付结果
```

>请求实例：http://yun.jfkj.xyz/userpay/coin.php?keeper=后台账号&api=应用API&user=用户账号&value=购买UY币数量&type=支付方式（wxpay/alipay/qqpay）
提示：这个支付请求必须要用网页来请求，你可以软件里写一个浏览器或者跳转浏览器都行。这个不是数据请求，把值填好转到WebView就可以。
 
----

* <font class="text-color-2" color="#e91e63">用户头像更新</font>：uyapi/uyyun_userhead.php
提交方式：POST

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
file（头像文件）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/uyyun_userhead.php?keeper=后台账号&api=应用API&user=用户账号&pass=用户密码&file=头像文件
 
----

* <font class="text-color-2" color="#e91e63">用户名称更新</font>：uyapi/user_newname.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
newname（新的用户名称）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/user_newname.php?keeper=后台账号&api=应用API&user=用户账号&pass=用户密码&newname=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户密码更新</font>：uyapi/user_newpass.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
newpass（新的用户密码）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/user_newpass.php?keeper=后台账号&api=应用API&user=用户账号&pass=用户密码&newpass=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户签名更新</font>：uyapi/user_newsign.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
 newsign（新的用户签名）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果
```

请求实例：http://yun.jfkj.xyz/uyapi/user_newsign.php?keeper=后台账号&api=应用API&user=用户账号&pass=用户密码&newsign=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户邮箱更新</font>：uyapi/user_newemail.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
newemail（新的用户QQ）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/user_newqq.php?keeper=后台账号&api=应用API&user=用户账号&pass=用户密码&newemail=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户用邮箱找回密码</font>：uyapi/user_forget_pass.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
newemail（用户邮箱）
返回数据：
code：true（成功）/false（失败）	
 msg=返回请求结果（账号数据会发到邮箱）
```

>请求实例：http://yun.jfkj.xyz/uyapi/user_forget_pass.php?keeper=后台账号&api=应用API&user=用户账号&newemail=用户收密码数据的邮箱
 
----


* <font class="text-color-2" color="#e91e63">所有资源列表</font>：uyapi/material_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果(这是公有列表，只会显示已经审核的所有该账户的资源列表)
title（资源标题）
content（资源内容）
img1（自定义数据）
img2（自定义数据）
img3（自定义数据）
sendtime（发布时间）
likenum（点赞的数量）
auther(资源发布者，管理员：官方；用户提交则是账号)
```

>请求实例：http://yun.jfkj.xyz/uyapi/material_list.php?keeper=后台账号&api=应用API
 
----

* <font class="text-color-2" color="#e91e63">用户点赞资源</font>：uyapi/material_like.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（赞者用户账号）
pass（用户密码）
id(资源id)
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果(一个月只能点赞一次，用户只能是本api内的用户)
```

>请求实例：http://yun.jfkj.xyz/uyapi/material_like.php?keeper=后台账号&api=应用API&user=用户账号&pass=用户密码&id=1
 
----

* <font class="text-color-2" color="#e91e63">用户提交资源</font>：uyapi/material_user_add.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
title（资源标题）
content（资源内容）
img1（可图片链接，或自定义数据）
img2（可图片链接，或自定义数据）
img3（可图片链接，或自定义数据）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果(后台审核过了才会显示在主列表，不通过则删除)
title（资源标题）
content（资源内容）
img1（自定义数据）
img2（自定义数据）
img3（自定义数据）
sendtime（发布时间）
likenum（点赞的数量）
auther(资源发布者，管理员：官方；用户提交则是账号)
```

>请求实例：http://yun.jfkj.xyz/uyapi/material_user_add.php?keeper=后台账号&api=应用API&user=用户账号&pass=用户密码&title=xxx&content=xxx&img1=xxx&img2=xxx&img3=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户私有资源列表</font>：uyapi/material_userself_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果(这是私有列表，会显示正在审核和已经审核的所有该账户提交的资源列表)
title（资源标题）
content（资源内容）
img1（自定义数据）
img2（自定义数据）
img3（自定义数据）
sendtime（发布时间）
likenum（点赞的数量）
auther(资源发布者，管理员：官方；用户提交则是账号)
```

>请求实例：http://yun.jfkj.xyz/uyapi/material_userself_list.php?keeper=后台账号&api=应用API&user=用户账号&pass=用户密码
 
----

* <font class="text-color-2" color="#e91e63">用户公有资源列表</font>：uyapi/material_user_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果(这是公有列表，只会显示已经审核的所有该账户的资源列表)
title（资源标题）
content（资源内容）
img1（自定义数据）
img2（自定义数据）
img3（自定义数据）
sendtime（发布时间）
likenum（点赞的数量）
auther(资源发布者，管理员：官方；用户提交则是账号)
```

>请求实例：http://yun.jfkj.xyz/uyapi/material_user_list.php?keeper=后台账号&api=应用API&user=用户账号
 
----

* <font class="text-color-2" color="#e91e63">用户删除私有资源</font>：uyapi/material_user_delete.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
id（资源ID）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果(只能删除已审核通过的资源，正在审核的不允许删除)
```

>请求实例：http://yun.jfkj.xyz/uyapi/material_user_delete.php?keeper=后台账号&api=应用API&user=用户账号&pass=用户密码&id=1
 
----

* <font class="text-color-2" color="#e91e63">资源社区查看</font>：uyapi/material_data.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
id（资源id）
返回数据：
code：true（成功）/false（失败）
 msg=返回请求结果
title（资源标题）
content（资源内容）
img1（自定义数据）
img2（自定义数据）
img3（自定义数据）
sendtime（发布时间）
likenum（点赞的数量）
auther(资源发布者，管理员：官方；用户提交则是账号)
```

>请求实例：http://yun.jfkj.xyz/uyapi/material_data.php?keeper=后台账号&api=应用API&id=资源id
 
----

* <font class="text-color-2" color="#e91e63">所有文章列表</font>：uyapi/article_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
title（文章标题）
content（文章内容，只返回前100个字符）
id （ID）
label（文章标签，多个标签用 | 分开，其他的自用）
sort（文章分类）
sendtime（发布时间）
flow（文章预览量，查看一次+1）
other(自定义数据)
coverimg（文章封面）
viparticle（是否会员文章，true【则只能会员用户查看】/false）
coinarticle（是否UY币文章，true/false）
coinnum （UY币数量，不是币文章则返回false）
```

>请求实例：http://yun.jfkj.xyz/uyapi/article_list.php?keeper=后台账号&api=应用API
 
----

* <font class="text-color-2" color="#e91e63">文章分类列表</font>：uyapi/article_sort_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
sort （文章分类名）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
title（文章标题）
content（文章内容，只返回前100个字符）
id （ID）
label（文章标签，多个标签用 | 分开，其他的自用）
sort（文章分类）
sendtime（发布时间）
flow（文章预览量，查看一次+1）
other(自定义数据)
coverimg（文章封面）
viparticle（是否会员文章，true【则只能会员用户查看】/false）
coinarticle（是否UY币文章，true/false）
coinnum （UY币数量，不是币文章则返回false）
```

>请求实例：http://yun.jfkj.xyz/uyapi/article_sort_list.php?keeper=后台账号&api=应用API&sort=xxx
 
----

* <font class="text-color-2" color="#e91e63">文章点赞</font>：uyapi/article_like.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user （用户账号）
pass（用户密码）
id（文章ID）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果（一个月只能一个赞）
```

>请求实例：http://yun.jfkj.xyz/uyapi/article_like.php?keeper=后台账号&api=应用API&user=123456&pass=123456&id=1
 
----

* <font class="text-color-2" color="#e91e63">用户文章查看</font>：uyapi/article_check.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user （用户账号）
pass（用户密码）
id（文章ID）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
title（文章标题）
content（文章内容）
id （ID）
label（文章标签，多个标签用 | 分开，其他的自用）
sort（文章分类）
sendtime（发布时间）
flow（文章预览量，查看一次+1）
other(自定义数据)
coverimg（文章封面）
viparticle（是否会员文章，true【则只能会员用户查看】/false）
coinarticle（是否UY币文章，true/false）
coinnum （UY币数量，不是币文章则返回false）
```

>请求实例：http://yun.jfkj.xyz/uyapi/article_check.php?keeper=后台账号&api=应用API&user=123456&pass=123456&id=1
提示：如果是UY币文章购买一次就可以，下载再请求此文章不会扣除用户uy币，而直接返回数据。（会员文章则不是，只能是会员才能看）
 
----

* <font class="text-color-2" color="#e91e63">文章搜索列表</font>：uyapi/article_search_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
title （文章标题关键词）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
title（文章标题）
content（文章内容，只返回前100个字符）
id （ID）
label（文章标签，多个标签用 | 分开，其他的自用）
sort（文章分类）
sendtime（发布时间）
flow（文章预览量，查看一次+1）
other(自定义数据)
coverimg（文章封面）
viparticle（是否会员文章，true【则只能会员用户查看】/false）
coinarticle（是否UY币文章，true/false）
coinnum （UY币数量，不是币文章则返回false）
```

>请求实例：http://yun.jfkj.xyz/uyapi/article_search_list.php?keeper=后台账号&api=应用API&title=xxx
 
----

* <font class="text-color-2" color="#e91e63">论坛系统</font> (模块-UID 帖子-PID 评论-ID)
应用模块列表：uyapi/forum_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
uid（模块ID）
icon（模块图标）
name（模块名）
content（模块介绍）
buildtime（创建时间）
adminuser（管理员用户账户 暂不可用）
other（自定义内容）
send (true/false 帖子是否需要审核)
sendif（true/false 该模块是否允许发帖）
```

>请求实例：http://yun.jfkj.xyz/uyapi/forum_list.php?keeper=后台账号&api=应用API
 
----

* <font class="text-color-2" color="#e91e63">模块单独数据</font>：uyapi/forum_data.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
icon（模块图标）
name（模块名）
content（模块介绍）
buildtime（创建时间）
adminuser（管理员用户账户 暂不可用）
other（自定义内容）
send (true/false 帖子是否需要审核)
sendif（true/false 该模块是否允许发帖）
```

>请求实例：http://yun.jfkj.xyz/uyapi/forum_data.php?keeper=后台账号&api=应用API&uid=1
 
----

* <font class="text-color-2" color="#e91e63">模块帖子列表</font>：uyapi/posts_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
outtype （列表返回方式，默认最新在前。asc/正序，最旧在前   desc/倒序，最新在前和默认空也如此  flow/按预览量 多的在前 like/按点赞，多的在前 comment/按评论数量，多的在前）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
id（帖子ID，也就是评论区需提交的pid）
user（发布用户账号）
name（发布用户名）
icon（发布用户头像）
title（帖子标题）
content（帖子内容）
img（帖子图片，或者自定义数据。我们不提供上传图功能，请自解决图床）
sendtime (帖子发布时间)
likenum（帖子点赞量）
flow（帖子访问量，点击调用posts_check.php接口才会自增）
label（帖子标签）
sort（帖子分类）
commentnum (帖子评论数量)
```

>请求实例：http://yun.jfkj.xyz/uyapi/posts_list.php?keeper=后台账号&api=应用API&uid=1&outtype=like
 
----

* <font class="text-color-2" color="#e91e63">帖子分类列表</font>：uyapi/posts_sort_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
sort （帖子分类名）
outtype （列表返回方式，默认最新在前。asc/正序，最旧在前   desc/倒序，最新在前和默认空也如此  flow/按预览量 多的在前 like/按点赞，多的在前 comment/按评论数量，多的在前）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
id（帖子ID，也就是评论区需提交的pid）
user（发布用户账号）
name（发布用户名）
icon（发布用户头像）
title（帖子标题）
content（帖子内容）
img（帖子图片，或者自定义数据。我们不提供上传图功能，请自解决图床）
sendtime (帖子发布时间)
likenum（帖子点赞量）
flow（帖子访问量，点击调用posts_check.php接口才会自增）
label（帖子标签）
sort（帖子分类）
commentnum (帖子评论数量)
```

>请求实例：http://yun.jfkj.xyz/uyapi/posts_sort_list.php?keeper=后台账号&api=应用API&uid=1&sort=xxx&outtype=like
 
----

* <font class="text-color-2" color="#e91e63">帖子搜索列表</font>：uyapi/posts_search.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
title（帖子标题关键是）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
id（帖子ID，也就是评论区需提交的pid）
user（发布用户账号）
name（发布用户名）
icon（发布用户头像）
title（帖子标题）
content（帖子内容）
img（帖子图片，或者自定义数据。我们不提供上传图功能，请自解决图床）
sendtime (帖子发布时间)
likenum（帖子点赞量）
flow（帖子访问量，点击调用posts_check.php接口才会自增）
label（帖子标签）
sort（帖子分类）
commentnum (帖子评论数量)
```

>请求实例：http://yun.jfkj.xyz/uyapi/posts_search.php?keeper=后台账号&api=应用API&uid=1&title=xxx

----

* <font class="text-color-2" color="#e91e63">模块帖子访问查看</font>：uyapi/posts_check.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
id （帖子ID）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
id（帖子ID，也就是评论区需提交的pid）
user（发布用户账号）
name（发布用户名）
icon（发布用户头像）
title（帖子标题）
content（帖子内容）
img（帖子图片，或者自定义数据。我们不提供上传图功能，请自解决图床）
sendtime (帖子发布时间)
likenum（帖子点赞量）
flow（帖子访问量，点击调用posts_check.php接口才会自增）
label（帖子标签）
sort（帖子分类）
commentnum (帖子评论数量)
```

>请求实例：http://yun.jfkj.xyz/uyapi/posts_check.php?keeper=后台账号&api=应用API&uid=1&id=1
 
----

* <font class="text-color-2" color="#e91e63">模块帖子发布</font>：uyapi/posts_add.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
user（发布用户账号）
pass（发布用户密码）
title（帖子标题）
content（帖子内容）
img（帖子图片，或者自定义数据。我们不提供上传图功能，请自解决图床）
label（帖子标签）
sort（帖子分类）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/posts_add.php?keeper=后台账号&api=应用API&uid=1&user=xxx&pass=xxx&title=xxx&content=xxx&img=xxx&label=xxx&sort=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户帖子列表</font>：uyapi/posts_user_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
user （发布者用户账号）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
id（帖子ID，也就是评论区需提交的pid）
user（发布用户账号）
name（发布用户名）
icon（发布用户头像）
title（帖子标题）
content（帖子内容）
img（帖子图片，或者自定义数据。我们不提供上传图功能，请自解决图床）
sendtime (帖子发布时间)
likenum（帖子点赞量）
flow（帖子访问量，点击调用posts_check.php接口才会自增）
label（帖子标签）
sort（帖子分类）
commentnum (帖子评论数量)
```

>请求实例：http://yun.jfkj.xyz/uyapi/posts_user_list.php?keeper=后台账号&api=应用API&uid=1&user=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户删除帖子</font>：uyapi/posts_delete.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
id （帖子ID）
user（帖子主用户账号）
pass（帖子主用户密码）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/posts_delete.php?keeper=后台账号&api=应用API&uid=1&id=1&user=xxx&pass=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户点赞帖子</font>：uyapi/posts_like.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
id （帖子ID）
user（点赞者用户账号）
pass（点赞者用户密码）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/posts_like.php?keeper=后台账号&api=应用API&uid=1&id=1&user=xxx&pass=xxx
 
----

* <font class="text-color-2" color="#e91e63">帖子评论列表</font>：uyapi/comment_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
pid （帖子ID）
outtype （输出方式，默认：最新序列。asc/正序（最久在前） desc（最新在前，默认也是））
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
id （评论ID）
user（评论者用户账号）
name（评论者用户名）
icon（评论者用户头像）
otheruser（被回复者用户账号）
othername（被回复者用户名）
othericon（被回复者用户头像）
sendtime （评论时间）
content （评论内容）
```

>请求实例：http://yun.jfkj.xyz/uyapi/comment_list.php?keeper=后台账号&api=应用API&uid=1&pid=1&id=1
提示：如果otheruser...三个参数只要一个是false ，那么这个是评论了帖子。【用户—》帖子】
如果三个参数不是false那么这个评论是回复了被回复者。【用户—》用户】
 
----

* <font class="text-color-2" color="#e91e63">评论给帖子</font>：uyapi/comment_posts.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
pid （帖子ID）
user（用户账号）
pass（用户密码）
content (评论内容)
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/comment_posts.php?keeper=后台账号&api=应用API&uid=1&pid=1&user=xxx&pass=xxx&content=xxx
提示：是直接评论到该帖子，而不是回复别人的评论。
 
----

* <font class="text-color-2" color="#e91e63">回复给帖子的评论</font>：uyapi/comment_matual.php
提交方式：POST/GET

```
提交参数：keeper（后台账号）
api（应用api）
uid (模块ID)
pid （帖子ID）
id （评论ID）
user（回复者用户账号）
pass（回复者用户密码）
otheruser （被回复者账号）
content (评论内容)
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/comment_matual.php?keeper=后台账号&api=应用API&uid=1&pid=1&id=1&user=xxx&pass=xxx&otheruser=xxx&content=xxx
提示：otheruser就是别人的账号，这不是评论，是回复给别人的评论。
 
----

* <font class="text-color-2" color="#e91e63">删除评论</font>：uyapi/comment_delete.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
pid （帖子ID）
id （评论ID，是自己的评论，否则删不了）
user（回复者用户账号）
pass（回复者用户密码）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/comment_delete.php?keeper=后台账号&api=应用API&uid=1&pid=1&id=1&user=xxx&pass=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户评论列表</font>：uyapi/comment_user_list.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
uid (模块ID)
pid （帖子ID）
user （评论者用户账户）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
id （评论ID）
user（评论者用户账号）
name（评论者用户名）
icon（评论者用户头像）
otheruser（被回复者用户账号）
othername（被回复者用户名）
othericon（被回复者用户头像）
sendtime （评论时间）
content （评论内容）
```

>请求实例：http://yun.jfkj.xyz/uyapi/comment_user_list.php?keeper=后台账号&api=应用API&uid=1&pid=1&id=1&user=xxx
 
----

* <font class="text-color-2" color="#e91e63">用户金币赠送</font>：uyapi/user_give_coin.php
提交方式：POST/GET

```
提交参数：
keeper（后台账号）
api（应用api）
user（用户账号）
pass（用户密码）
coinnum （金币数量）
otheruser （对方账号）
返回数据：
code：true（成功）/false（失败）
msg=返回请求结果
```

>请求实例：http://yun.jfkj.xyz/uyapi/user_give_coin.php?keeper=后台账号&api=应用API&user=xxx&pass=xxx&coinnum=1&otheruser=xxx



**来自[](https://jfkj.xyz)🚨🧻作者Evan的编辑❤🅱**