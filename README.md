# Python-12-
Python学习笔记(12)
# p41 流程控制语句break
''''从键盘录入密码，如果正常就结束循环，如果正确就跳出循环'''
for item in range(3):
    pwd=input('请输入密码')
    if pwd=='8888':
        print('密码正确')
        break
    else:
        print('密码错误')

a=0
while a<3:
    pwd=input('请输入密码')
    if pwd=='8888':
        print('密码正确')
        break
    else:
        print('密码错误')
'''改变变量'''
a+=1 #while循环这里一定要注意变量的递增



# p42 流程控制语句continue
'''要求输出1到50之间所有5的倍数,要求使用continue实现'''
for item in range(1,51):
    if item%5==0:
        print(item)

print('--------------使用continue实现------------------')
for item in range(1,51):
    if item%5!=0:
        continue
    print(item)



# p43 else语句
#else语句有三种搭配情况：1.与if判断句搭配   2.与while循环语句搭配(当while循环完就执行else语句)   3.与for循环搭配
for item in range(3):
    pwd=input('请输入密码:')
    if pwd=='8888':
        print('密码正确')
        break
    else:
        print('密码错误')
else:  #这里的else与for循环搭配
    print('对不起，三次密码均错误')

a=0
while a<3:
    pwd=input('请输入密码')
    if pwd=='8888':
        print('密码正确')
        break
    else:
        print('密码错误')
    ‘’‘改变变量’‘’
    a+=1
else:
    print('对不起，三次密码均错误')
