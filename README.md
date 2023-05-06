# Plotting by Class - on Matplot Library
# Create a class Circle
    
    import matplotlib.pyplot as plt
    %matplotlib inline

class Circle(object):    
# Constructor = to show attributes of the circle
    
    def __init__(self, radius, color):
        self.radius = radius
        self.color = color 
        
# Method for drawing
    
    def drawCircle(self):
        plt.gca().add_patch(plt.Circle((0, 0), radius=self.radius, fc=self.color))
        plt.axis('scaled')
        plt.show()   
        
## Ex. Radius is 1, and the color is 'red', we can write,
    radius = 1
    color = 'red'
    Redcircle = circle(1,'red')
    Redcircle.drawCircle() #This is the drawing code

