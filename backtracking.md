```
PrintWriter Out = new PrintWriter(new File("buckets.out"));
Out.printf("%d\n", ans);
Out.close();

int bx, by, rx, ry, lx, ly;
```
Proper subset

empty: 0, 1, 2, 3, 4
flying: 1, 2, 4
telpathic: 2
spots: 3, 4

Backtracking algorith

Depth-first search, Breadthfirst search, Dijkstra Algorithm, Flood-fill

bag -- container clase -- vector, arraylist, map, set, queue
```
put the starting stone into your bag
while(bag.has_stone()) {
    pick a stone from the bag
	check stone's property
	foreach (direction)
	    if it's a new direction {
		    push current stone into your bag
			move down the direction
		}
	}	
}
```