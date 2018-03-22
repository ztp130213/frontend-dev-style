参考：
[airbnb js编码风格](http://airbnb.io/javascript/)
[google js编码风格](https://google.github.io/styleguide/jsguide.html)

采用eslint验证代码格式

### 1.命名
#### 1.1 声明前使用var,let,const等，一行声明一个，不用逗号分隔。
#### 1.2 变量一般采用驼峰式命名。
#### 1.3 变量命名规则 最好是具象的，布尔值需要带 is,has,can, 单位值需要带_ms,_s,_px 等

bad code
```
height
let read = false
```
good code
```
height_px
let isRead = false
```
#### 1.4 常量采用大写字母加"_"连接。
#### 1.5 构造函数采用首字母大写驼峰式，一般方法名采用驼峰式。 

### 2.空格

运算符，{，}，(，)前后留空格。

### 3.缩进
#### 3.1 缩进采用两个空格。
#### 3.2 单行长度不超过120个字符。

### 4.注释

文件注释
```
/*
 * @file xxx 
 * @desc xxx
 */
```

类注释

```
/*
 * @class xxx 
 * @desc xxx
 */
```

函数/方法注释

```
/*
 * @desc xxx 
 * @param {string} xxx
 * @param {number} xxx
 * @return {number} xxx
 */
```

### 5.分号使用

不使用分号

### 6.函数

函数参数不超过5个。（超过5个用objectType代替）

### 7.异常

#### 7.1 允许使用try/catch
#### 7.2 上线代码不允许使用debugger，console，alert等关键字。

### 8.逻辑控制

#### 8.1 分支超过5个的判断使用switch case，switch case需要带default。
#### 8.2 判断条件过长，使用变量标识
#### 8.3 判断使用严格类型判断0,null,undefined,固定字符使用===。

### 9.原型

#### 9.1 禁止对顶级对象进行原型修改。
#### 9.2 原型不允许保存属性，只能保存方法，因为子类会互相影响。


