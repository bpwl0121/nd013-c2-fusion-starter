# report of midterm
## Find and display 10 examples of vehicles with varying degrees of visibility in the point-cloud.
In the first image, the black, red and yellow boxes all show vehicles traveling in the opposite direction to the lidar. 

The black box shows the vehicle very close to the side of the lidar, and only part of the point cloud of the vehicle is shown.

The red is close to the lidar, but within the appropriate lidar detection range, almost the entire vehicle's point cloud is shown. And the point cloud of the vehicle in the yellow box is blocked by other vehicles.

The blue box shows the same direction of travel as the lidar sensor, but this is a rare point cloud of a car with a trailer.
<img src="img/1.PNG"/>

The green box shows the same driving direction as the lidar sensor, but these point clouds are farther away from the lidar sensor, so the point cloud is less dense and does not show the complete car point cloud.
<img src="img/2.PNG"/>
The purple box below shows the point cloud image of the vehicle farther to the side of the lidar sensor.
<img src="img/3.PNG"/>

The black box below shows the point cloud image of the closer vehicle on the side of the lidar sensor. The blue box shows the point cloud of the closer vehicle with the trailer.
<img src="img/4.PNG"/>

### In summary, the point cloud information of the lidar sensor is related to the distance of the vehicle, the relative position of the vehicle and the sensor (considered only from the point cloud map, without considering weather effects). For example, for a vehicle on the side of the sensor, we do not know information about the other side of the vehicle.

## Identify vehicle features that appear as a stable feature on most vehicles (e.g. rear-bumper, tail-lights) and describe them briefly. Also, use the range image viewer from the last example to underpin your findings using the lidar intensity channel.

The bumper can be clearly identified in the point cloud and intensity map.
<img src="img/bumper_pcl.PNG"/>
<img src="img/bumper_int.PNG"/>
The range image also confirms this:
<img src="img/5.PNG"/>
### We can also prove this from the point cloud diagram in the first question. lidar sensors in their work generally detect the front and rear of other vehicles. And the front and rear bumpers and headlights are its obvious features.