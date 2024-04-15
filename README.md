import turtle
t = turtle.Turtle()
radius = int(input("Enter radius: "))
number = int(input("Enter size: "))
peddals = int(input("Enter number of peadels: "))
many = int(input("Enter number of flowers: "))
far = int(input("How far apart: "))
t.speed(100)
r=radius
n=number
t.penup()
# t.forward(100)
# t.right(180)
t.pendown()
for i in range(many):
  for i in range(peddals):
    t.fillcolor("pink")
    t.begin_fill()
    t.right(45)
    for i in range(1, n + 1, 1):
      t.circle(r * i)
    t.end_fill()
  t.penup()
  t.forward(far)
  t.pendown()
