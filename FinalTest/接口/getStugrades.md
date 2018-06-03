``<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

接口：getStugrades
--
  [点击返回](../README.md)\
用例： [学生成绩查询](../用例/学生成绩查询.md)

- 功能：
    帮助学生查询实验成绩。

- 权限：
    学生

- API请求地址：
    接口基本地址/v1/api/getStugrades

- 请求方式 ：
    GET
- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |Stu_id|学生的学号|

- 返回实例：

        {
            "status": true,
            "infor": null,
            "ID":"201510414104",
            "name":"cxz",
            "class_name":"软件工程1班"
            "grades":"88"
            "Tea_evaluate":"实验不错"
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|布尔类型，true表示正确的返回，false表示有错误|
  |infor|返回查询结果信息|
  |ID|学生学号|
  |name|学生姓名|
  |class_name|班级|
  |grades|实验成绩|



