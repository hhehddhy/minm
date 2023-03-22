# minm
"""
练习题，华氏温度转换为摄氏温度
提示：华氏温度到摄氏温度的转换公式为：C=(F-32)/1.8
"""
#f = float(input('请输入华氏温度值：'))
#c = (f -32)/1.8
#print('%.1f华氏度 = %.1f摄氏度' % (f, c))#占位符这个还是不怎么懂，其中%d是整数的占位符，%f是小数的占位符，%%表示百分号

"""
输入圆的半径计算计算周长和面积
周长=2*π*r ，面积=π*r*r 
"""
#r = float(input('请输入圆的半径：'))
#l = 2*3.14*r
#area = 3.14*r*r
#print('周长: %.2f' % l)
#print('面积: %.2f' % area)

"""
输入年份判断是不是闰年
需要满足以下条件中的任意一个： ① 该年份能被4 整除同时不能被100 整除； ② 该年份能被400整除
"""
#year = float(input('请输入年份：'))
#leap_year = year % 4 == 0 and year % 100 != 0 or year % 400 == 0  #%取模，这里为什么要取模你，不能直接除？
#print(leap_year)

"""
练习1：英制单位英寸与公制单位厘米互换。
1 厘米[cm]	10 mm	0.3937 英寸[in]

2 百分制成绩转换为等级制成绩。
要求：如果输入的成绩在90分以上（含90分）输出A；80分-90分（不含90分）输出B；70分-80分（不含80分）输出C；60分-70分（不含70分）输出D；60分以下输出E。

练习3：输入三条边长，如果能构成三角形就计算周长和面积。

"""
"""
x =float(input('输入值：'))
if x > 1:
    y = 3*x -5
elif x >= -1:
    y = x+2
else :
    y = 5*x +3
print('f(%.2f) = %.2f' % (x ,y))


value = float(input('请输入数值：'))
unit = input('请输入单位：')
if unit == 'cm' or unit == '厘米':
    print('%f厘米 = %f英寸' % (value , value / 2.45))
elif unit == 'in' or  unit =='英寸':
    print('%f英寸 = %f厘米' % (value , value * 2.45))
else:
    print('输入错误')


from operator import indexOf


score = float(input('输入分数：'))
if score >= 90:
    print('A')
elif score >=80:
    print('B')
elif score >=70:
    print('c')
else:
    print('请重新输入')
"""

s = 127
is_sushu = True
for i in range(2,s-1):
    if s%i==0 :
        print('not',i)
        is_sushu=False
print(is_sushu)
print(min(3,6))
