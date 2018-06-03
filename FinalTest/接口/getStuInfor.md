<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getStuInfor
  [点击返回](../README.md)\
用例： [用户信息](../用例/用户信息.md)\
     [用户列表](../用例/用户列表.md)

- 功能：
    查看用户的详细信（只有教师能查看），查看用户的列表（所有人都能看得见）。

- 权限：
    学生和老师。

- API请求地址：
    接口基本地址/v1/api/getStuInfor

- 请求方式 ：
    GET

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |Stu_id|学生的学号或者教师的工号|

- 返回实例：

        {
            "status": true,
            "infor": null,
            "ID":"201510414104",
            "name":"cxz",
            "class_name":"软件工程1班"
            "github_username":"cxz",
            "type":"学生"
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|布尔类型，true表示正确的返回，false表示有错误|
  |infor|返回查看结果信息|
  |ID|学生学号或者教师工号|
  |name|用户姓名|
  |class_name|工作单位名称|
  |github_username|gitHub用户名|
  |type|用户类型：老师或者学生|