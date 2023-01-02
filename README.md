# area_of_different_shapes
import math

def circle_area(radius):
    return math.pi * (radius ** 2)

def triangle_area(base, height):
    return 0.5 * base * height

def square_area(length,width):
    return length * width

asking_for_shape = input("enter your shape (square,triangle or circle: ")

if asking_for_shape == "circle":
    radius = float(input("give me radius: "))
    print(f"your circle area is {circle_area(radius)}")
elif asking_for_shape == "triangle":
    base = float(input("give me base: "))
    height = float(input("give me height: "))
    print(f"your triangle area is {triangle_area(base, height)}")
elif asking_for_shape == "square":
    length = float(input("give me length: "))
    width = float(input("give me width: "))
    print(f"your square area is {square_area(length,width)}")
else:
    print(f"I don't have your area of {asking_for_shape}.")
