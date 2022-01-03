# UDWA
UDWA:UAV Dataset with Altitude



## Download

| Part | URL | DOI |
| --- | --- | --- |
| Place01-Place15 | [https://zenodo.org/record/5813232#.YdKDG2BByUk](https://zenodo.org/record/5813232#.YdKDG2BByUk) | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5813232.svg)](https://doi.org/10.5281/zenodo.5813232) |
| Place16-Place30 | [https://zenodo.org/record/5813236#.YdKDJWBByUk](https://zenodo.org/record/5813236#.YdKDJWBByUk) | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5813236.svg)](https://doi.org/10.5281/zenodo.5813236) |
| Place31-Place39 | [https://zenodo.org/record/5813325#.YdKDImBByUk](https://zenodo.org/record/5813325#.YdKDImBByUk) | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5813325.svg)](https://doi.org/10.5281/zenodo.5813325) |



## Collection Platform

We use [Mavic Air 2](https://www.dji.com/mavic-air-2) and [DJI Fly](https://www.dji.com/dji-fly) to capture the video stream required by the dataset. Mavic Air 2 is a compact and portable drone. The most important thing is that its primary camera with 12 million pixels can capture high-definition video with a resolution of 3840×2160 at a rate of 60 frames per second. And DJI Fly is its supporting flight control software, which can control the drone while viewing the real-time images collected by its camera, which is very helpful for the scene selection and altitude control. 



## Dataset Description

- The UAV Dataset with Altitude (*UDWA*) contains 179 original video clips, each of which is about 4 minutes and 50 seconds, and the total video length is about 13 hours. Finally, we extracted it to 46028 images in `.jpg` format.
- We shot all videos on sunny days in Kunming, Yunnan, and Maitreya, Yunnan.
- We chose 6 flight altitudes, which are 50 meters, 60 meters, 70 meters, 80 meters, 90 meters, and 100 meters. To focus on the different altitudes, the horizontal position under one location will not change. There are only six certain altitudes, and the camera's downward inclination angle remains unchanged at 45 degrees.
- We selected 39 different places for shooting and divided the data of different places. These places are mainly schools, subway stations, commercial streets, and tourist attractions.  
- Moreover, all pictures extracted from the video maintain a high resolution of 3840×2160, and no down-sampling is performed. The original video is 30fps. According to the actual speed of the object to be detected, the first frame of each second is selected as the extracted picture. 



## Dataset Annotation

Unlike a large number of classification categories in most data, the use scenarios of the system are mainly road and pedestrian monitoring, and the attention is focused on people and cars that often move.

So the tags of the dataset have only two categories: **person** and **car**. What needs to be explained here is that in the classification, both pedestrians and people riding on vehicles belong to **person**. All four-wheeled and three-wheeled vehicles belong to **car**, but bicycles and motorcycles do not belong to this category. 

To complete the self-adaptation system, we selected four places with fewer goals and marked a total of 2866 pictures. Each of these pictures contains about 10-50 marker boxes, and most of them include objects of two categories simultaneously.

It takes about 5 minutes on average to mark such a picture. We carry out 8 hours of marking a day and finally complete the marking of 2866 pictures in 30 days.

The annotation tool we used is [CVAT](https://github.com/openvinotoolkit/cvat). And to facilitate the use of more people, the annotation file adopts the standard coco format.

We will continue to annotate other pictures and use them for future research. 


| Scenario| Annotions | 50M | 60M | 70M | 80M | 90M | 100M |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Scenario1 | [instances_place02.json](annotations/instances_place02.json) | ![](/assets/images/place02-50M-DJI_0276-00121.jpg.jpg) | ![](/assets/images/place02-60M-DJI_0275-00058.jpg.jpg) |  ![](/assets/images/place02-70M-DJI_0274-00287.jpg.jpg) |  ![](/assets/images/place02-80M-DJI_0274-00179.jpg.jpg) |  ![](/assets/images/place02-90M-DJI_0274-00026.jpg.jpg) |  ![](/assets/images/place02-100M-DJI_0274-00016.jpg.jpg) |
| Scenario2 | [instances_place06.json](annotations/instances_place06.json) | ![](/assets/images/place06-50M-DJI_0295-00182.jpg.jpg) | ![](/assets/images/place06-60M-DJI_0292-00021.jpg.jpg) |  ![](/assets/images/place06-70M-DJI_0294-00263.jpg.jpg) |  ![](/assets/images/place06-80M-DJI_0294-00215.jpg.jpg) |  ![](/assets/images/place06-90M-DJI_0293-00136.jpg.jpg) |  ![](/assets/images/place06-100M-DJI_0294-00060.jpg.jpg) |
| Scenario3 | [instances_place22.json](annotations/instances_place22.json) | ![](/assets/images/place22-50M-DJI_0367-00184.jpg.jpg) | ![](/assets/images/place22-60M-DJI_0367-00254.jpg.jpg) |  ![](/assets/images/place22-70M-DJI_0368-00183.jpg.jpg) |  ![](/assets/images/place22-80M-DJI_0369-00276.jpg.jpg) |  ![](/assets/images/place22-90M-DJI_0370-00164.jpg.jpg) |  ![](/assets/images/place22-100M-DJI_0371-00077.jpg.jpg) |
| Scenario4 | [instances_place27.json](annotations/instances_place27.json) | ![](/assets/images/place27-50M-DJI_0392-00078.jpg.jpg) | ![](/assets/images/place27-60M-DJI_0392-00255.jpg.jpg) |  ![](/assets/images/place27-70M-DJI_0393-00154.jpg.jpg) |  ![](/assets/images/place27-80M-DJI_0394-00121.jpg.jpg) |  ![](/assets/images/place27-90M-DJI_0394-00269.jpg.jpg) |  ![](/assets/images/place27-100M-DJI_0395-00279.jpg.jpg) |


Figure above presents the example of *UDWA*, which includes four scenarios and each contains the annotated information from 50 meters to 100 meters.



## Dataset Splits
The 2866 annotated pictures are divided with 8:2 into the training set and validation set. We call the remaining unlabeled pictures the test-challenge set. The final training set contains 2290 pictures, the validation set contains 576 pictures, and the test-challenge set contains 43162 pictures. These pictures are divided according to 50 meters, 60 meters, 70 meters, 80 meters, 90 meters, 100 meters, which is convenient for testing the accuracy and other performance at different altitudes. 
