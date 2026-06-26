# pytest-api-test-framework
项目介绍：该项目是一个在线购物的商城网站，包括用户注册，登录，下单，上架/下架商品，下单支付等相关功能,主要针对该网站搭建了接口自动化框架,封装了相关请求,实现接口关联,结果断言,数据库断言等脚本；

技术栈(自动化)：Python+pytest+sqlalchemy+requests+allure+jsonpath+yaml+Jenkins+Linux

项目架构：
- 项目采用pytest单元测试框架来管理用例，使用pytest.ini结合conftest.py来配置|管理用例执行规则；
- 采用json提取器以及yaml的方式来存放接口配置参数，实现case与参数的分离，实现了用例解耦；
- 使用assert关键字断言接口返回结果以及状态码，数据库断言等，保证了用例的可靠性以及稳定性；
- 采用POM模式分离用例层与驱动层，实现了用户管理，商品下单全流程的用例，使脚本兼容性更佳；
- 使用yaml的方式来构造请求，包括请求头，请求体，token，url等，使用parametrize来读取请求参数；
