

# Python 點產生器

以下 Python 腳本會為多個範例產生點陣列。請將這些腳本貼至 Python 腳本節點，如下所示：

![](images/12-10/PythonPointGenerators_01.png)

**python_points_1**

```
out_points = []

for i in range(11):
sub_points = []
for j in range(11):
z = 0
if (i == 5 and j == 5):
z = 1
elif (i == 8 and j == 2):
z = 1
sub_points.Add(Point.ByCoordinates(i, j, z))
out_points.Add(sub_points)

OUT = out_points
```

**python_points_2**

```
out_points = []

for i in range(11):
z = 0
if (i == 2):
z = 1
out_points.Add(Point.ByCoordinates(i, 0, z))

OUT = out_points
```

**python_points_3**

```
out_points = []

for i in range(11):
z = 0
if (i == 7):
z = -1
out_points.Add(Point.ByCoordinates(i, 5, z))

OUT = out_points
```

**python_points_4**

```
out_points = []

for i in range(11):
z = 0
if (i == 5):
z = 1
out_points.Add(Point.ByCoordinates(i, 10, z))

OUT = out_points
```

**python_points_5**

```
out_points = []

for i in range(11):
sub_points = []
for j in range(11):
z = 0
if (i == 1 and j == 1):
z = 2
elif (i == 8 and j == 1):
z = 2
elif (i == 2 and j == 6):
z = 2
sub_points.Add(Point.ByCoordinates(i, j, z))
out_points.Add(sub_points)

OUT = out_points
```

