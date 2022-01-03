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

| ![place01](/assets/images/raw/place01-50M-DJI_0271-00001.jpg) | ![place02](/assets/images/raw/place02-50M-DJI_0276-00117.jpg) | ![place03](/assets/images/raw/place03-50M-DJI_0276-00273.jpg) | ![place04](/assets/images/raw/place04-50M-DJI_0281-00001.jpg) | ![place05](/assets/images/raw/place05-50M-DJI_0286-00011.jpg) | ![place06](/assets/images/raw/place06-50M-DJI_0291-00090.jpg) | ![place07](/assets/images/raw/place07-50M-DJI_0296-00001.jpg) | ![place08](/assets/images/raw/place08-50M-DJI_0301-00001.jpg) |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| ![place09](/assets/images/raw/place09-50M-DJI_0303-00001.jpg) | ![place10](/assets/images/raw/place10-50M-DJI_0308-00001.jpg) | ![place11](/assets/images/raw/place11-50M-DJI_0313-00001.jpg) | ![place12](/assets/images/raw/place12-50M-DJI_0318-00001.jpg) | ![place13](/assets/images/raw/place13-50M-DJI_0323-00001.jpg) | ![place14](/assets/images/raw/place14-50M-DJI_0329-00001.jpg) | ![place15](/assets/images/raw/place15-50M-DJI_0334-00001.jpg) | ![place16](/assets/images/raw/place16-50M-DJI_0339-00001.jpg) |
| ![place17](/assets/images/raw/place17-50M-DJI_0344-00001.jpg) | ![place18](/assets/images/raw/place18-50M-DJI_0348-00001.jpg) | ![place19](/assets/images/raw/place19-50M-DJI_0352-00001.jpg) | ![place20](/assets/images/raw/place20-50M-DJI_0357-00001.jpg) | ![place21](/assets/images/raw/place21-50M-DJI_0362-00001.jpg) | ![place22](/assets/images/raw/place22-50M-DJI_0367-00003.jpg) | ![place23](/assets/images/raw/place23-50M-DJI_0373-00001.jpg) | ![place24](/assets/images/raw/place24-50M-DJI_0377-00001.jpg) |
| ![place25](/assets/images/raw/place25-50M-DJI_0383-00001.jpg) | ![place26](/assets/images/raw/place26-50M-DJI_0388-00001.jpg) | ![place27](/assets/images/raw/place27-50M-DJI_0392-00001.jpg) | ![place28](/assets/images/raw/place28-50M-DJI_0397-00001.jpg) | ![place29](/assets/images/raw/place29-50M-DJI_0402-00001.jpg) | ![place30](/assets/images/raw/place30-50M-DJI_0407-00001.jpg) | ![place31](/assets/images/raw/place31-50M-DJI_0411-00001.jpg) | ![place32](/assets/images/raw/place32-50M-DJI_0415-00001.jpg) |
| ![place33](/assets/images/raw/place33-50M-DJI_0420-00001.jpg) | ![place34](/assets/images/raw/place34-50M-DJI_0425-00001.jpg) | ![place35](/assets/images/raw/place35-50M-DJI_0430-00001.jpg) | ![place36](/assets/images/raw/place36-50M-DJI_0434-00001.jpg) | ![place37](/assets/images/raw/place37-50M-DJI_0438-00001.jpg) | ![place38](/assets/images/raw/place38-50M-DJI_0443-00001.jpg) | ![place39](/assets/images/raw/place39-50M-DJI_0447-00001.jpg) |  |


## Dataset Annotation

Unlike a large number of classification categories in most data, the use scenarios of the system are mainly road and pedestrian monitoring, and the attention is focused on people and cars that often move.

So the tags of the dataset have only two categories: **person** and **car**. What needs to be explained here is that in the classification, both pedestrians and people riding on vehicles belong to **person**. All four-wheeled and three-wheeled vehicles belong to **car**, but bicycles and motorcycles do not belong to this category. 

We first selected four places with fewer goals and marked a total of 2866 pictures. Each of these pictures contains about 10-50 marker boxes, and most of them include objects of two categories simultaneously.

It takes about 5 minutes on average to mark such a picture. We carry out 8 hours of marking a day and finally complete the marking of 2866 pictures in 30 days.

The annotation tool we used is [CVAT](https://github.com/openvinotoolkit/cvat). And to facilitate the use of more people, the annotation file adopts the standard coco format.

We will continue to annotate other pictures and use them for future research. 


| Scenario | Annotions | 50M | 60M | 70M | 80M | 90M | 100M |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Scenario1 | [instances_place02.json](annotations/instances_place02.json) | ![Scenario1-50m](/assets/images/annotated/place02-50M-DJI_0276-00121.jpg.jpg) | ![Scenario1-60m](/assets/images/annotated/place02-60M-DJI_0275-00058.jpg.jpg) |  ![Scenario1-70m](/assets/images/annotated/place02-70M-DJI_0274-00287.jpg.jpg) |  ![Scenario1-80m](/assets/images/annotated/place02-80M-DJI_0274-00179.jpg.jpg) |  ![Scenario1-90m](/assets/images/annotated/place02-90M-DJI_0274-00026.jpg.jpg) |  ![Scenario1-100m](/assets/images/annotated/place02-100M-DJI_0274-00016.jpg.jpg) |
| Scenario2 | [instances_place06.json](annotations/instances_place06.json) | ![Scenario2-50m](/assets/images/annotated/place06-50M-DJI_0295-00182.jpg.jpg) | ![Scenario2-60m](/assets/images/annotated/place06-60M-DJI_0292-00021.jpg.jpg) |  ![Scenario2-70m](/assets/images/annotated/place06-70M-DJI_0294-00263.jpg.jpg) |  ![Scenario2-80m](/assets/images/annotated/place06-80M-DJI_0294-00215.jpg.jpg) |  ![Scenario2-90m](/assets/images/annotated/place06-90M-DJI_0293-00136.jpg.jpg) |  ![Scenario2-100m](/assets/images/annotated/place06-100M-DJI_0294-00060.jpg.jpg) |
| Scenario3 | [instances_place22.json](annotations/instances_place22.json) | ![Scenario3-50m](/assets/images/annotated/place22-50M-DJI_0367-00184.jpg.jpg) | ![Scenario3-60m](/assets/images/annotated/place22-60M-DJI_0367-00254.jpg.jpg) |  ![Scenario3-70m](/assets/images/annotated/place22-70M-DJI_0368-00183.jpg.jpg) |  ![Scenario3-80m](/assets/images/annotated/place22-80M-DJI_0369-00276.jpg.jpg) |  ![Scenario3-90m](/assets/images/annotated/place22-90M-DJI_0370-00164.jpg.jpg) |  ![Scenario3-100m](/assets/images/annotated/place22-100M-DJI_0371-00077.jpg.jpg) |
| Scenario4 | [instances_place27.json](annotations/instances_place27.json) | ![Scenario4-50m](/assets/images/annotated/place27-50M-DJI_0392-00078.jpg.jpg) | ![Scenario4-60m](/assets/images/annotated/place27-60M-DJI_0392-00255.jpg.jpg) |  ![Scenario4-70m](/assets/images/annotated/place27-70M-DJI_0393-00154.jpg.jpg) |  ![Scenario4-80m](/assets/images/annotated/place27-80M-DJI_0394-00121.jpg.jpg) |  ![Scenario4-90m](/assets/images/annotated/place27-90M-DJI_0394-00269.jpg.jpg) |  ![Scenario4-100m](/assets/images/annotated/place27-100M-DJI_0395-00279.jpg.jpg) |


Figure above presents the example of *UDWA*, which includes four scenarios and each contains the annotated information from 50 meters to 100 meters.
