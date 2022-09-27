# Matplotlib-2D-Graph
# python library Matplotlib
import numpy as np
import matplotlib.pyplot as plt
#x value

x = np.array([80, 85, 90, 95, 100, 105, 110, 115, 120, 125])

#y value

y = np.array([240, 250, 260, 270, 280, 290, 300, 310, 320, 330])

#cursive font style
#x,y Heading colors
#x,y Heading Size

font1 = {'family':'Cursive','color':'blue','size':14}
font2 = {'family':'Cursive','color':'red','size':10}

#loc used to put the heading i center,left,right

plt.title("Graph", fontdict = font1,loc='center')
plt.xlabel("X Heading", fontdict = font2)
plt.ylabel("Y Heading", fontdict = font2)

#using dot marking

plt.scatter(x, y)

#inside the graph square using grid

plt.grid(color = 'green',linestyle = '--', linewidth = '0.4')

#show the graph

plt.show() 
