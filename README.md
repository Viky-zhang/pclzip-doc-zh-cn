
# 简介
阅读：https://vikyd.gitbooks.io/pclzip/content/

PHP 库 [PclZip](http://www.phpconcept.net/pclzip) 的中文文档（非官方）。





# 译注：PclZip 是什么？
PclZip 是一个 PHP 库，用于解压或压缩 Zip 压缩包。
 
不同于 PHP 自带的`ZipArchive + getNameIndex`、`zip_open + zip_read + zip_entry_name`（基于 C++），
PclZip 采用纯 PHP 的解决方案，可避免一些 PHP 自带的 zip 方便的 bug（如对 zip 压缩包内含 GBK 编码的文件名的识别问题）。





# 使用方式
通常有两种使用方式：
1. 直接下载`pclzip.lib.php`，在你的 PHP 文件顶部添加`include_once(__DIR__ . '/pclzip/pclzip.lib.php');`。
1. 使用 Composer 引用 PclZip，引入方式，在命令行执行：`composer require pclzip/pclzip`（非官方，但文件相同）。



# 目录
* [介绍](top/home.md)

* [用户指南](user_guide/introduction.md)
  * [如何使用](user_guide/how_it_works.md)
  * [可选参数](user_guide/optional_arguments.md)
  * [异常处理](user_guide/error_handling.md)
  * [自定义 PclZip](user_guide/customizing_pclzip.md)
  * [Bug 定位](user_guide/troubleshooting_pclzip.md)
  * [ZIP 格式](user_guide/zip_format.md)

* [类和方法](class_methods/home.md)
  * [PclZip::PclZip()](class_methods/pclzip.md)
  * [PclZip::create()](class_methods/create.md)
  * [PclZip::listContent()](class_methods/list_content.md)
  * [PclZip::extract()](class_methods/extract.md)
  * [PclZip::properties()](class_methods/properties.md)
  * [PclZip::add()](class_methods/add.md)
  * [PclZip::delete()](class_methods/delete.md)
  * [PclZip::merge()](class_methods/merge.md)
  * [PclZip::duplicate()](class_methods/duplicate.md)
  

* [常见问题](top/faq.md)

* [最新消息](top/news.md)

* [更新日志](top/release_notes.md)

* [下载](top/downloads.md)


# 完善
水平有限，难免错漏。

问题意见，欢迎提 PR：https://github.com/vikyd/pclzip-doc-zh-cn.git


不定时更新。


# 相关资源
## 使用
- [PclZip 官网](http://www.phpconcept.net/pclzip)
- [PclZip GitHub（非官方）](https://github.com/ivanlanin/pclzip)
- [PclZip Compose（非官方）](https://packagist.org/packages/pclzip/pclzip)

# 使用 PclZip 的项目
至少有以下项目用到了 PclZip：
- [WordPress](https://github.com/WordPress/WordPress/blob/master/wp-admin/includes/class-pclzip.php)
- [PHPExcel](https://github.com/ddeboer/phpexcel/blob/master/Classes/PHPExcel/Shared/PCLZip/pclzip.lib.php)
- [Drupal](https://www.drupal.org/project/pclzip)
- [Stackoverflow 相关问题](http://stackoverflow.com/search?tab=votes&q=pclzip)


> 建议尽量阅读 PclZip 官方英文文档
 
