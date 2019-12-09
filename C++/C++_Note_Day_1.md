

```c++
#include <iostream>
#include <stdio.h>
using namespace std;

int main(void){
    // 1 :
    //float r, phi = 5,3.14159;   OUTPUI: Wrong
    //float r = 5, phi = 3.14159;   OUTPUT: 5.000000\n3.141590
    // printf("%f\n",r);
    // printf("%f",phi);
    
    // 2 : 数据类型 float 单精度 double 双精度浮点型
    // double r, phi  = 3.14159;
    // scanf("%lf",&r);
    // printf("A=%.4lf",r*r*phi);
    // return 0;
    
    // 3 : C++ cin cout
    double r,phi = 3.14159;
    cin>>r;
    printf("A=%.4lf",r*r*phi);
}
```

## 浮点类型

下表列出了关于标准浮点类型的存储大小、值范围和精度的细节：

| 类型        | 存储大小 | 值范围                 | 精度      |
| :---------- | :------- | :--------------------- | :-------- |
| float       | 4 字节   | 1.2E-38 到 3.4E+38     | 6 位小数  |
| double      | 8 字节   | 2.3E-308 到 1.7E+308   | 15 位小数 |
| long double | 16 字节  | 3.4E-4932 到 1.1E+4932 | 19 位小数 |



## I/O 库头文件

下列的头文件在 C++ 编程中很重要。

| 头文件     | 函数和描述                                                   |
| :--------- | :----------------------------------------------------------- |
| <iostream> | 该文件定义了 **cin、cout、cerr** 和 **clog** 对象，分别对应于标准输入流、标准输出流、非缓冲标准错误流和缓冲标准错误流。 |
| <iomanip>  | 该文件通过所谓的参数化的流操纵器（比如 **setw** 和 **setprecision**），来声明对执行标准化 I/O 有用的服务。 |
| <fstream>  | 该文件为用户控制的文件处理声明服务。我们将在文件和流的相关章节讨论它的细节。 |





\605. 简单乘积

```c++
#include <iostream>
#include <stdio.h>
using namespace std;

int main(void){
    int var_1,var_2,PROD;
    //scanf("%d%d",&var_1,&var_2);
    cin>>var_1>>var_2;
    PROD = var_1 * var_2;
    printf("PROD = %d",PROD);
    return 0;
}
```

