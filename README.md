import turtle

# Set up the screen
screen = turtle.Screen()
screen.title("i call this bow")
screen.bgcolor("white")

# Create a turtle for drawing
bow = turtle.Turtle()
bow.speed(2)
bow.color("black")
bow.width(3)

# Function to draw the bow
def draw_bow():
    # Draw the bow body
    bow.circle(100, 180)  #this thing is a create half circele 
    bow.left(90) # this a thing turn left  
    bow.forward(201)  # this thing go down 201  
# Draw the bow
draw_bow()

# below down this is arrow  

# Set up the screen
screen = turtle.Screen()
screen.title("arrow")
screen.bgcolor("white")

# Create a turtle for drawing
arrow = turtle.Turtle() 
arrow.speed(2) # arrow speed 
arrow.color("gold") # changes color 
arrow.width(2) #turtle pen size 

# Function to draw a horizontal line
def draw_horizontal_line(length): 
    arrow.forward(length) 

# Function to draw a triangle
def draw_triangle(size):
    for _ in range(3):
        arrow.forward(size)
        arrow.right(120) #turn right 120 

# Draw a horizontal line
arrow.penup()
arrow.goto(-90, 90) # goes to middle bow and create a horizontal line 
arrow.pendown()
draw_horizontal_line(200) # draw a line 200 

# Draw a triangle at the end of the line
arrow.penup()
arrow.goto(110, 80) #create triangle end of the horizontal line 
arrow.left(90)
arrow.pendown()
draw_triangle(20) #size of triangle 

# Hide the turtle and display the result
arrow.hideturtle()
turtle.done()


