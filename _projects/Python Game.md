---
title: "Simple two-player game"
excerpt: "A two player game programmed in python in parallel with a final research paper on gaming<br/>"
collection: projects
---

In support of my final paper written for WRI115: Systems of Play, I programmed a simple two player game in which players must compete using the same keyboard, arrow keys or WASD, in order to fight for a randomly moving red square. The concept of the game was kept simple in order to showcase the effects of randomly generated elements that are used to draw attention in popular video games. <br/>
<img src="/images/dda.png" height="500" width="500"> <br/>
The code was written to be very simple and clean as I made use of inheritance and OOP for each of the interactable objects in the game such as the player and the collectable red squares. Essentially, each type of interatable object had an x y and color whose attributes would be inherited to other objects such as the points and the player with their own respective functions. 
```python
class block(character):
    def __init__(self, x, y, color):
        self.x = x
        self.y = y
        self.color = color

    def random(self):
        self.x = random.randint(0, gridnum-1) * gap
        self.y = random.randint(0, gridnum-1) * gap
```
