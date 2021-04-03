# 建立第一个cpp文件
## 以及VIM编辑器的初使用
### 进入root账号
* 登陆的时候用户名输入root，密码输入之前使用的用户名的密码      
（为了接下来的配置，配置完成后登陆平时的用户名即可）

### 检查gcc，g++的配置
* 打开终端，输入       
```
yum -y install gcc
yum -y install gcc-c++
```
* 检查是否成功
```
which gcc
which g++
```

### 建立一个Cpp文件     
* 第一种方式——文本编辑器        
  1.打开文本编辑器，写代码            
    ```
    #include<iostream>
    using namespace std;
    int main()
    {
        cout << "hello linux" << endl;
        return 0;
    }
    ```
  2.保存文件，后缀改成.cpp, hello.cpp           
  
  3.记住保存文件的位置，例如 /root/cpp         
  
  4.打开终端输入cd命令切换至cpp文件所在处       
    `cd /root/cpp/hello `     
     cpp文件名（不带后缀）       
     
  5.编译命令
    `g++ hello.cpp -o resname`        
    g++：cpp 用 g++，C 用 gcc     
    要编译的文件名(带后缀)             
    -o :          
    resname:编译后文件的命名，不带后缀（理解成exe文件吧，仅用于分辨加不加后缀！与原理无关）         
    
  6.运行文件
    ` ./resname `

    
  * 第二种方式——VIM编辑器       
   输入` vim hello.cpp `          
   创建了一个cpp文件进入vim编辑器     

   一开始是命令模式     
   点击‘insert’按键或者‘i'按键进入编辑模式    

   输入代码     

   按’ESC'退出编辑模式重新进入命令模式     
   然后输入冒号` :wq `      
   退出vim编辑器

   编译和运行文件步骤同第一种方法
   ```
   g++ hello.cpp -o hello
   ./hello
   ```
 
 
    
    
