# UJM TIV
`UJM TIV` is a material dataset consist of images of 11 material classes `aluniminum foil`, `brown bread`, `corduroy`, `cork`, `cotton`, `cracker`, `lettuce leaf`, `linen`, `white bread`, `wood` and `wool`. Each image is a 20x20 RGB image. All of these categories are also presented in [KTH-TIPS2 Dataset](https://www.csc.kth.se/cvaatabases/kth-tips/credits.html). `UJM TIV` stands for `University Jean Monnet, Texture Under Varying Illumination, Pose and Viewing`. Our `UJM TIV` dataset provides images with higher intra class variability. Images were captured using `4 viewing (frontal/90°, 10°, 30°, 60°)` and `4 Lighting (frontal/90°, 20°, 45°, 65°)` conditions and 2 sample orientation in a controlled acquisition setup. 

Here is an example of a sample from 11 differnt categories:
![Sample Images](imgs/sample_imgs.PNG)
In the above image `a. aluniminum foil`, `b. brown bread`, `c. corduroy`, `d. cork`, `e. cotton`, `f. cracker`, `g. lettuce leaf`, `i. linen`, `j. white bread`, `k. wood` and `l. wool`.

Each view folder contains images of 11 material categories captured with specific viewing and lighting conditions. The viewing and lighting conditions for the selected view images are shown in the following image:
![View Image](imgs/view_image_conditions.PNG)

The image acquisition setup is schemetically depicted in the image below. For the sake of our studies, the plane bounded by vectors N and I was positioned
perpendicular to the plane bounded by vectors N and V.
<img src= "imgs/acquisition_conditions.PNG" width="650" height="500">

![Results Image](imgs/exp_results.PNG)

In this research we introduced multi-view learning solution for the material classification which clearly outperformed the traditional single view based deep learning solution which can be observed from above table. We employed a two branched siamese network which takes input from two different views and extract specific informattion from each views. In the end the extracted features are fusioned togather. The architecture of the proposed solution is shown in the image below. Our paper can be accessed online [Multi-view Learning for Material Classification](https://www.mdpi.com/2313-433X/8/7/186)

![Siamese Architecture](imgs/siamese_architecture.PNG)

To split the views into train, test and validation folders [Python Split folders](https://github.com/jfilter/split-folders) module can be used.

If you use UJM TIV in a scientific publication, we would appreciate references to the following paper:
## [Multi-view Learning for Material Classification](https://www.mdpi.com/2313-433X/8/7/186)

Biblatex entry:
```
@article{sumon2022multi,
  title={Multi-View Learning for Material Classification},
  author={Sumon, Borhan Uddin and Muselet, Damien and Xu, Sixiang and Tr{\'e}meau, Alain},
  journal={Journal of Imaging},
  volume={8},
  number={7},
  pages={186},
  year={2022},
  publisher={MDPI}
```
