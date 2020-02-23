# blog 
# my  blog
# 环境 PHP环境 apache  ， MySQL 
# public/index   "192.168.192.129"自改
# 把blog.sql  导入自己的数据库
# 框架  think PHP 5.0
# 后台默认密码  123456

流程
一.下载php5.0  在官网下载www.thinkphp.cn
    解压后有
      application      文件夹/项目主目录 
      extend           文件夹/拓展
      public           文件夹/入口文件
      runtime          文件夹/项目运行时的临时文件
      thinkphp         文件夹/项目的主要配置文件，栗汝  database.php连接数据库
      vendor           文件夹/我也不知道干嘛用的
      .gitgnore        GITGNORE文件
      bulid.php        PHP Script
      composer.json    JSON文件
      composer.lock    LOCK文件
      think            文件
      README.md        自述文档
      LICENSE.txt      文本文档
2.分离模板
      前台写3个通用模板  头  尾  右     后台写两个模板  头  左
3.连接数据库    
   创建数据库
   数据库名   blog
   字符集     utf8
   排序规则   utf8_general_ci
   
   创建数据表
   表1  tp_admin    id(主键)   username  password
   表2  tp_article  id(主键)   title     author    desc   keywords    content     pic    click     state(bull)  time   cateid
   表3  tp_cate     id(主键)   catename
4.管理员后台登陆
    调用admin模块   输入用户名  密码  和数据库进行比对   访问控制登录后台  登陆入口  admin/login.html
5.栏目添加及唯一验证           //栏目名写入数据库   并进行查重
6.文章添加  导入UEditor插件    //添加文章导入数据库  

    
    
    
