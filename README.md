# VS-code-Python

## input형
```PYTHON
target = input("고백하고 싶은 대상은 누구입니까? ")
expression = input("대상을 한마디로 표현한다면? ")
felling = input("대상에 대한 감정은 무엇인가요? ")

print("="*25)
print("*"*10, " 나의 비밀스런 고백 ", "*"*7)
print("나의 %s %s님!"%(expression, target))
print("나의 {0}하는 마음을 받아주세요!".format(felling))
print("="*25)
```

## %f쓰는 식 
```PYTHON
x = float(input("첫번째 값: "))
y = float(input("두번째 값: "))

print("%f + %f = %.2f"%(x, y, x + y))
print("%f - %f = %.2f"%(x, y, x - y))
print("%f * %f = %.2f"%(x, y, x * y))
print("%f / %f = %.2f"%(x, y, x / y))
```

## turtle형
```PYTHON
import turtle

color = turtle.textinput("Color", "도형의 선색을 입력하시오. (영어)")
fill = turtle.textinput("색채우기", "도형에 색 채우기를 할까요? (Y/N)")
shape = int(turtle.textinput("도형", "몇각형 도형을 원합니까?"))

if color:
    turtle.pencolor(color)
else:
    turtle.pencolor("black")

if fill == "Y" or "y":
    turtle.fillcolor(color)
else:
    turtle.fillcolor('white')

turtle.begin_fill()
for i in range(shape):
    turtle.forward(12)
    turtle.right(360/shape)
turtle.end_fill()
```

## turtle 사용해서 여러 도형 만들기
```PYTHON
import turtle

turtle.pencolor("black")


turtle.fillcolor('blue')
turtle.begin_fill()
turtle.setposition(0,0)

for i in range (3):
    turtle.forward(50)
    turtle.right(360/3)
turtle.penup()

turtle.end_fill()

turtle.begin_fill()
turtle.fillcolor('yellow')
turtle.setposition(100, 0)
turtle.pendown()
for i in range (4):
    turtle.forward(50)
    turtle.right(360/4)
turtle.penup()
turtle.end_fill()

turtle.fillcolor('red')
turtle.begin_fill()
turtle.setposition(200,0)
turtle.pendown()
for i in range (5):
    turtle.forward(50)
    turtle.right(360/5)
turtle.penup()
turtle.end_fill()

turtle.fillcolor('green')
turtle.begin_fill()
turtle.setposition(300,0)
turtle.pendown()

for i in range (6):
    turtle.forward(50)
    turtle.right(360/6)

turtle.end_fill()
```

## 추가
```
************************************************
       python... 알아서 생각 하는 수 밖에..
************************************************
