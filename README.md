# 闲聊编程中的命名方法

## 命名方法

### 约定一：驼峰命名法（Camel case）
单词之间没有空格。除第一个单词外，每个单词都以大写字母开头。
例如：camelCase, myVariableName, myUrl, getUsers, beforeBodyWrite, returnType
这可能是使用最广泛的约定。它可以在 JavaScript、Java、C++、C# 等语言中找到。

### 约定二： 帕斯卡命名法（Pascal case）
单词之间没有空格。每个单词都以大写字母开头。
举例：PascalCase, MyVariableName, MyUrl, GetUsers, RuntimeException，AppVersion
这个惯例在 Pascal 编程语言中使用，或者在 Java、PHP 中用来命名类。

### 约定三： 烤串命名法（Kebab case）
单词用小写，用连字符（-）连接。
举例：kebab-case, my-variable-name, background-color
推荐使用烤烤串命名法来编写 URL 和 URL 中的参数，以及为图片、PDF 和其它网络文件命名。在编程中，例如，它被用来命名 HTML 和 CSS 代码中的类和 ID。

### 约定四：蛇形命名法（Snake case）
单词用小写（或大写），用下划线连接。
举例：snake_case, my_variable_name, DEFAULT_LANGUAGE，ROOT_PATH
在 PHP、Ruby 和 Python 中使用了蛇形命名法。这个约定有一个变体，即所有的单词都大写，用下划线分隔（例如：MY_CONSTANT_NAME）。多数语言的常量名称都使用这种形式。大写小写这两种变体可以分别表述为大蛇形（BIG_SNAKE_CASE）和小蛇形（small_snake_case）。

### 如此：

1. 目录和文件
  - 目录使用小蛇形命名（small_snake_case）；
  - 类的文件名均以命名空间定义，并且命名空间的路径和类库文件所在路径一致；
  - 类（包含接口和 Trait）文件采用帕斯卡命名（PascalCase），其它文件采用小蛇形命名（small_snake_case）；
  - 类名（包括接口和 Trait）和文件名保持一致，统一采用帕斯卡命名（PascalCase）；
2. 函数和类、属性命名
  - 类的命名采用帕斯卡命名法（PascalCase），例如 User、ResponseEntity；
  - 函数的命名使用小蛇形（small_Snake_case）的方式，例如 get_client_ip；
  - 方法的命名使用驼峰法（camelCase），例如 getUserName；
  - 属性的命名使用驼峰法（camelCase），例如 tableName、instance；
  - 特例：以双下划线__打头的函数或方法作为魔术方法，例如 __call 和 __autoload；
3. 常量和配置
  - 常量以大蛇形命名（BIG_SNAKE_CASE），例如 APP_PATH；
  - 配置参数以小蛇形命名（small_snake_case），例如 url_route_on 和 url_convert；
  - 环境变量定义使用大蛇形命名（BIG_SNAK_CASE），例如 APP_DEBUG；
4. 数据表和字段
  - 数据表和字段采用小蛇形命名（small_snake_case），并注意字段名不要以下划线开头，例如 think_user 表和 user_name 字段，不建议使用驼峰和中文作为数据表及字段命名。

