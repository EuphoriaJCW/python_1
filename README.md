# python_1
感想：由于本人纯粹是零基础，导致开始前一两个月全部在学习语法，感觉很重要的是掌握一些内置函数，能帮助我们很高效的写出代码，后面一段时间开始学习贪心，动态规划和搜索，难度陡然增加，基本上是力求把平时每周的作业搞懂，然后额外会去刷一些leetcode和晴问上的题，感觉还是能学到很多东西的。
代码
1.判断闰年（http://cs101.openjudge.cn/practice/02733/）
a=int(input())
if a%4!=0:
    print('N')
elif a%3200==0:
    print('N')
elif a%100==0 and a%400!=0:
    print('N')
else:
    print('Y')
2.鸡兔同笼（http://cs101.openjudge.cn/practice/02750/）
a=int(input())
if a%2!=0:
    print('0 0')
elif a%2==0 and a%4!=0:
    b=(a+2)/4
    c=a/2
    print(int(b),int(c))
else:
    b=a/4
    c=a/2
    print(int(b),int(c))
3.Domino piling（http://codeforces.com/problemset/problem/50/A）
M,N=list(map(int,input().split()))
s=M*N//2
print(s)
4.Theatre and square（https://codeforces.com/problemset/problem/1/A）
n,m,a=list(map(int,input().split()))
x=(n+a-1)//a
y=(m+a-1)//a

s=x*y
print(s)
5.Petya and strings（http://codeforces.com/problemset/problem/112/A）
string1=input()
string2=input()
string1_=string1.lower()
string2_=string2.lower()
if string1_<string2_:
    print('-1')
elif string1_==string2_:
    print('0')
else:
    print('1')
6.Team（http://codeforces.com/problemset/problem/231/A）
n=int(input())
ls=[]
m=0
for i in range(n):
    ls.append(list(map(int,input().split())))
for each in ls:
    if each[0]+each[1]+each[2]>=2:
        m+=1
    else:
        m+=0
print(m)


