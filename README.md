# packagetest-for-laravel5
laravel5.6 扩展包开发 DEMO 


1、安装
  ```
  composer update qiang/packagetest-for-laravel
  ```

2、添加服务,修改 config/app.php
  --配置服务，在providers数组最下面添加：
  ```
    Qiangzi\Packagetest\PackagetestServiceProvider::class
  ```
  --配置别名，在aliases数组最下面添加：
  ```
    Qiangzi\Packagetest\Facades\Packagetest::class
  ```
3、执行以下命令，同步数据
  ```
    composer dump-autoload
  ```
4、发布资源文件
  ```
    php artisan vendor:publish –provider=”Aex\Packagetest\PackagetestServiceProvider” 
  ```
5、安装完成。
