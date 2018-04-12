内容

* 完成权限管理，完成管理员权限的登录界面，并显示显示学生的信息

步骤

1. 新建类 \*\*domain-&gt;UserLogin\*\*，此类对应于数据库中的userlogin表；
2. 新建接口 \*\*persistence-&gt;UserLoginMapper\*\*，此接口中实现\*\*getUserLogin\*\*方法；然后新建xml文件\*\*UserLoginMapper.xml\*\*，实现方法\*\*getUserLogin\*\*的SQL实现；
3. 新建类 \*\*service-&gt;LoginService\*\*，实现\*\*getUserByNameAndPwd\*\*方法，此方法调用\*\*UserLoginMapper\*\*中的\*\*getUserLogin\*\*方法；
4. 新建类\*\*controller-&gt;LoginController\*\*，调用\*\*LoginService\*\*中的\*\*getUserByNameAndPwd\*\*方法。



