# 111111
def f(x):
    return(-x**2+3*x-2)
h=0.1
a=1
b=2
print( "###f(x)=-x^2+3*x-2 from a=1 to b=2###" )
for x in range(a,b+1):
    print("when x =",x,"=> f(x)",f(x))
    x+=h
first=f(1)
last=f(2)
print(first)
print(last)
x=a+h
middlesum=0
while x<b:
    middlesum +=f(x)
    x+=h
ApproxValue=h/2*(first+last+middlesum)
ture=1/6
error=(ture-ApproxValue)/ture*100
print(ApproxValue)
print(error,"%")
