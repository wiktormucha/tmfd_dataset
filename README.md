# TriModal Face Detection Dataset - TMFD Dataset


![TMFD Example](/images/tmfd_example.png "TMFD frame example")

[![DOI](https://zenodo.org/badge/DOI/10.1145/3523111.3523114.svg)](https://doi.org/10.1145/3523111.3523114)

TMFD Dataset addresses the lack of available depth and thermal face detection benchmarks. The corresponding depth and thermal data frames accompany each RGB image in the dataset. 
The dataset encompasses a wide range of variations. The samples include different numbers of people in the scene, different individuals, various types of backgrounds, varying distances of measurement, and wearable accessories worn by the individuals, such as hoodies, headphones, hats, glasses, and face masks. Additionally, the dataset includes different types of illumination in the scene. The dataset is categorized into three separate groups based on the complexity and difficulty level of face detection. The first subset represents the easiest detection conditions, with images containing a single person against a simple background. The sensor is positioned close to the target. This subset consists of 781 images for each modality.
The second group represents medium detection conditions. The sensor placement remains the same as in the first subset, but additional variety is introduced. Individuals are captured wearing accessories that serve as obstacles to make detection more challenging. These accessories include hoodies, headphones, hats, and glasses. The second group also includes images with multiple persons in the scene to test the performance of multiple face detection. There are 965 images for each modality in this group.
The last group represents the most challenging images for detection. In this case, the sensor is placed further away from the target. The scenes feature various obstacles, such as computer screens, plants, desks, and chairs, with individuals interacting with them. The presence of singular and plural individuals is also included. A distinct subset within this collection consists of images from a previous, easier scene, but with the addition of face mask usage to increase the difficulty of the prediction task. This particular group contains 1062 images for each modality.

## Folder structure
<pre>
TMFD Dataset
|--images
|   |--easy
|   |   |--d
|   |   |   |--easy_d_1.png
|   |   |   |-- ...
|   |   |--rgb
|   |   |   |--easy_rgb_1.png
|   |   |   |--...
|   |   |--t
|   |   |   |--easy_t_1.png
|   |   |   |--...
|   |--medium
|   |--hard
|--labels
|   |--easy
|   |   |--easy_1.txt
|   |   |-- ...
|   |--medium
|   |--hard
</pre>

## Labels description

Example label:

```
362 232 389 277
459 205 491 250
```
Each line represents bounding box for one face. If there is no bounding box, image does not contain any face. All given bounding boxes are in scale of images 640x480 pixels.


## Download 
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7994645.svg)](https://doi.org/10.5281/zenodo.7994645)


## Terms of Use and Citation Request

This database may be used for non-commercial research purpose only. If you publish material based on this database, we request you to include a reference to:



```
@inproceedings{mucha2022depth,
author = {Mucha, Wiktor and Kampel, Martin},
title = {Depth and Thermal Images in Face Detection - A Detailed Comparison Between Image Modalities},
year = {2022},
isbn = {9781450395670},
url = {https://doi.org/10.1145/3523111.3523114},
doi = {10.1145/3523111.3523114},
booktitle = {2022 the 5th International Conference on Machine Vision and Applications (ICMVA)},
pages = {16–21},
numpages = {6},
location = {Singapore, Singapore},
series = {ICMVA 2022}
}
```


Further details regarding camera calibration and setup can be found in the publication below:
```
@inproceedings{strohmayer2022A,
author = {Strohmayer, Julian and Kampel, Martin},
title = {A Compact Tri-Modal Camera Unit for RGBDT Vision},
year = {2022},
isbn = {9781450395670},
url = {https://doi.org/10.1145/3523111.3523116},
doi = {10.1145/3523111.3523116},
booktitle = {2022 the 5th International Conference on Machine Vision and Applications (ICMVA)},
pages = {34–42},
numpages = {9},
location = {Singapore, Singapore},
series = {ICMVA 2022}
}
```