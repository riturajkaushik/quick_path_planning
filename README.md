# Quick path planning
 
 * **A-star algorithm**
 
    - start position, goal position, obstacles and map boundary can take any float values. The algorithm automatically segments the space according to the given resolution. 
 
 ```python
    obstacles = [[-4, -1, -3, 10], [2.5, 5.0,-8, 5]] #Rectangular obstacles [xmin, xmax, y min, ymax]
    boundary = [-10, 10, -10, 10] #Map boundary [xmin, xmax, ymin, ymax]
    planner = A_star(obstacles, boundary, resolution=0.8)
    start, goal = [-7,0], [7,5]
    path = planner.plan(start, goal)
 ```
    -  Path planning can also be visualised
