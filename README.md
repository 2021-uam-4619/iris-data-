import pandas as pd
import numpy as pn
import matplotlib.pyplot as plt
import statistics as state
d=pd.read_csv('Iris.csv')
d

plt.plot(d.SepalLengthCm.head(),d.SepalWidthCm.head(),color='red')

plt.barh(d.PetalLengthCm.head(),d.PetalWidthCm.head(),color=['r','g','b','y','m'])

colors=[1,2,3,4,5]

plt.scatter(d.PetalLengthCm.head(),d.PetalWidthCm.head(),c=colors)

print("mean of adjusted_satisfaction=",state.mean(d.SepalWidthCm))

print("median of adjusted_satisfaction=",state.median(d.PetalLengthCm))

f=plt.axes(projection="3d")

colors=[1,2,3,4,5,6,7,8,9,10]

f.scatter3D(d.SepalLengthCm(10),d.petalWidth.head(10),c=colors,cmap="cool")


f.view_init(0,10)

f=plt.axes(projection="3d")

f.plot3D(d.sepalLengthcm.head(),d.sepalWidthCm.tail(),lw=4)


#lw used for bolt

colors=[1,2,3,4,5]

plt.scatter(d.SepalLengthCm.head(),d.SepalWidthCm.head(),c=colors)

plt.colorbar(label="asim",extend='both',shrink=1,pad=0.12,format="%.3f")#when give arrow shape use extend function

plt.clim(1,10)#given couting of color bar

#shrink use bar size change

#pad use graph size change


#when take foemate of bar using format function

