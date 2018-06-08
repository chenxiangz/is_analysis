<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：setStugrades
[返回](../README.md) \
用例： [学生成绩管理](../用例/学生成绩管理.md)

- 功能：
    教师针对学生提交的实验项目，做出修改，提交做出的评价和成绩。


- 权限：
    老师：可以批改所有学生的实验作业。

- API请求地址：
    接口基本地址/v1/api/setStugrades

- 请求方式 ：
    POST

- 请求实例：
        {
            "course_id":"1",
            "student_id": "201510414104",
            "test_total": 60,
            "test_data": [
                {
                "test_id":5,
                "test_result": 80,
                "test_evaluate":"本次实验的不足。。。。。。",
                }
            ]
        }

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |course_id|课程编号|
  |stu_id|学号|
  |total|本次批改的所有实验的总数，小于等于全部实验的总数|
  |test_data|实验的成绩和评语|
  |test_id|实验编号|
  |test_result|本实验成绩，可以为空，为空表示没有批改。|
  |test_evaluate|本实验老师的评价，可以为空|

- 返回实例：

        {
            "status": true,
            "infor": null
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|布尔类型，true表示正确的返回，false表示有错误|
  |infor|返回结果说明信息|


