接口：addTeaInfor
--------------
 [点击返回](../README.md)   \
用例： [添加教师信息](../用例/添加教师信息.md)
- 功能：
    添加新教师的各种信息。

- 权限：
    只有使用管理员权限时，才能进行添加等操作。

- API请求地址：
    接口基本地址/v1/api/addTeaInfor

- 请求方式 ：
    POST

- 请求实例：

        {
            "teacher_id":"01010",
            "teacher_name":"zwd",
        }

- 请求参数说明:

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |teacher_id|教师的工号|
  |teacher_name|教师姓名|

- 返回实例：

        {
            "status": true,
            "infor": null,
        }

- 返回参数说明：

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |status|布尔类型，true表示正确的返回，false表示有错误|
  |info|返回添加结果信息|