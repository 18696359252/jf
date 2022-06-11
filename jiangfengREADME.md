
#include<stdio.h>
int main()
{
    int x, y, z;
    char c;
    printf("格式为：数据运算符数据\n");
    printf("请输入：");
    scanf_s("%d%c%d", &x, &c, 1, &y);//在vs2017中输入字符型变量需要定义长度否则出错
    switch (c)
    {
    case '+':
        z = x + y;
        break;
    case '-':
        z = x - y;
        break;
    case '*':
        z = x * y;
        break;
    case '/':
        z = x / y;
        break;
    default:
        printf("erro!");
        break;
    }
    printf("%d", z);
    return 0;
}
