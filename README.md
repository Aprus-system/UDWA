# UDWA
UDWA:UAV Dataset with Altitude

# Download
| Part | URL | DOI |
| --- | --- | --- |
| Place01-Place15 | [https://zenodo.org/record/5813232#.YdKDG2BByUk](https://zenodo.org/record/5813232#.YdKDG2BByUk) | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5813232.svg)](https://doi.org/10.5281/zenodo.5813232) |
| Place16-Place30 | [https://zenodo.org/record/5813236#.YdKDJWBByUk](https://zenodo.org/record/5813236#.YdKDJWBByUk) | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5813236.svg)](https://doi.org/10.5281/zenodo.5813236) |
| Place31-Place93 | [https://zenodo.org/record/5813325#.YdKDImBByUk](https://zenodo.org/record/5813325#.YdKDImBByUk) | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5813325.svg)](https://doi.org/10.5281/zenodo.5813325) |

# Collection Platform
We use [Mavic Air 2](https://www.dji.com/mavic-air-2) and [DJI Fly](https://www.dji.com/dji-fly) to capture the video stream required by the dataset. Mavic Air 2 is a compact and portable drone. The most important thing is that its primary camera with 12 million pixels can capture high-definition video with a resolution of 3840×2160 at a rate of 60 frames per second. And DJI Fly is its supporting flight control software, which can control the drone while viewing the real-time images collected by its camera, which is very helpful for the scene selection and altitude control. 

# Dataset Description
- The UAV Dataset with Altitude (*UDWA*) contains 179 original video clips, each of which is about 4 minutes and 50 seconds, and the total video length is about 13 hours. Finally, we extracted it to 46028 images in `.jpg` format.
- We shot all videos on sunny days in Kunming, Yunnan, and Maitreya, Yunnan.
- We chose 6 flight altitudes, which are 50 meters, 60 meters, 70 meters, 80 meters, 90 meters, and 100 meters. To focus on the different altitudes, the horizontal position under one location will not change. There are only six certain altitudes, and the camera's downward inclination angle remains unchanged at 45 degrees.
- We selected 39 different places for shooting and divided the data of different places. These places are mainly schools, subway stations, commercial streets, and tourist attractions.  
- Moreover, all pictures extracted from the video maintain a high resolution of 3840×2160, and no down-sampling is performed. The original video is 30fps. According to the actual speed of the object to be detected, the first frame of each second is selected as the extracted picture. 
