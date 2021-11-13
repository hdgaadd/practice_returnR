# 统一返回结果集

**作用：** 对每次url调用返回的结果做统一处理，返回的R对象可以**显示在页面上**，起到给前端页面提示的作用

**步骤：**

- 触发控制层，结果返回一个R对象，而该R对象传递的参数是服务层返回的对象

  return R.ok(userService.updateUserInfo(userDto));

**页面接收到的为：**

- {"code":1,"data":{"id":1,"name":"Jone","age":18,"email":"[test1@baomidou.com](mailto:test1@baomidou.com)"},"message":"success"}