### 1，fork 这个项目

  使用 github ci需要。

### 2, 配置参数

  在 https://github.com/{fork的仓库地址}/settings/secrets/actions
里添加相应的值。

参数如下

| key    | value                    |
| ------ | ------------------------ |
| sid    | openid对应的学号         |
| openid | we重邮上的 openid        |
| name   | 姓名                     |
| sex    | 男/女                    |
| addr1  | 默认重庆市,重庆市,南岸区 |
| addr2  | 默认重庆邮电大学###      |
| stutype| 适配本科生和研究生的接口 默认研究生，研究生 yjs 本科生bks|
| hookurl| 企业微信hookurl，推送结果用，可不填|

### 3，修改定时任务

https://github.com/kaiili/checkinapi/blob/master/.github/workflows/checkin-main.yml#L9

  修改即可。
