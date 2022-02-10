# Photi-LakeIce Dataset

This is a repository dedicated for the Photi-LakeIce dataset described in the papers:<br>

>[Ice Monitoring in Swiss Lakes from Optical Satellites and Webcams using Machine Learning (Tom et.al., 2020)](https://www.mdpi.com/2072-4292/12/21/3555)<br>
>[Lake Ice Monitoring with Webcams and Crowd-​Sourced Images (Prabha et.al., 2020)](https://www.isprs-ann-photogramm-remote-sens-spatial-inf-sci.net/V-2-2020/549/2020/isprs-annals-V-2-2020-549-2020-relations.html)

## What this repo contains?
1. [Link](https://share.phys.ethz.ch/~pf/tommdata/Dataset.tar.xz) to download the Photi-LakeIce dataset (876 MB, 4017 images) with (a) RGB webcam images, (b) pixel-wise ground truth annotations
2. [Link](https://share.phys.ethz.ch/~pf/tommdata/Pre-trained_Model.tar.xz) to download the [Deep-U-Lab](https://www.isprs-ann-photogramm-remote-sens-spatial-inf-sci.net/V-2-2020/549/2020/isprs-annals-V-2-2020-549-2020-relations.html) model (146 MB) pre-trained on Photi-LakeIce datset
3. Details about the Photi-LakeIce dataset


## Dataset details

### Folder structure 
  ```bash
├── dataset
    ├── lake
        ├── winter
            ├── camera
                ├── data
                ├── labels
├── readme.txt
```
### Naming convention for each image in the 'Data' and 'Labels' folders
Lake_camera_year_monthdate_hour_minute.jpg (Lake Sihl images)
example: Sihl_Cam2_2016_1221_10_07.jpg
Lake_camera_year_monthdate_hour_minute.png (Lake StMoritz images)
example: StMoritz_Cam1_2016_1221_10_07.png

### Ground truth annotation (4 Class) 
- ice
- snow
- water
- clutter

### Two winters included
- 2016-17 
- 2017-18

### Lakes included
- Sihl (47.1370° N, 8.7801° E) located in Canton Schwyz, Switzerland
- St. Moritz (46.4942° N, 9.8449° E) located in Canton Graubuenden, Switzerland

### Cameras
- 2 from lake St. Moritz (Camera 0, Camera 1)
- 1 from lake Sihl (Camera 2)

<img src="figures/Dataset_figures.png" />

### Example images
![](figures/Example_images.png)

### Texture variability
<img src="figures/Texture_variablity.png" width=500/>

### Class imbalance
<img src="figures/Class_imbalance.png"/>

## Some results from [Tom et.al. (2020)](https://www.mdpi.com/2072-4292/12/21/3555) and [Prabha et.al. (2020)](https://www.isprs-ann-photogramm-remote-sens-spatial-inf-sci.net/V-2-2020/549/2020/isprs-annals-V-2-2020-549-2020-relations.html)

### Qualitative results
<img src="figures/Example_results_Qualitative.png"/>

### Quantitative results
![](figures/Example_results_Quantitative.png)

### Timeline results
![](figures/Example_results_Timeline.png)

### Precision-Recall curves
![](figures/Example_results_PRcurve.png)

## Citation
Kindly cite our papers, if you use this dataset in your work:

> @article{tom_prabha_2020:isprs,<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;author    = {Manu Tom and Rajanie Prabha and Tianyu Wu and Emmanuel Baltsavias and Laura Leal-Taixe and Konrad Schindler},<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title     = {Ice Monitoring in Swiss Lakes from Optical Satellites and Webcams Using Machine Learning},<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;journal   = {Remote Sens.},<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;year      = {2020},<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;volume    = {12},<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;issue     = {21},<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pages     = {3555},<br>
}   

>@article{prabha_tom_2020:isprs,<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;author={Prabha, R. and Tom, M. and Rothermel, M. and Baltsavias, E. and Leal-Taixe, L. and Schindler, K.},<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title={Lake Ice Monitoring with Webcams and Crowd-Sourced Images},<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;booktitle={ISPRS Ann. Photogramm. Remote Sens. Spatial Inf. Sci.},<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;year={2020},<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;volume={V-2-2020},<br>
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pages={549–556},<br>
>}

## Related links
1. Multi-sensor lake ice monitoring with machine (deep) learning. [Project github page](https://github.com/czarmanu/lake-ice-ml).
2. Lake ice monitoring with webcams and crowd-sourced images with Deep-U-Lab. [Github repo (tensorflow code, pre-trained model)](https://github.com/czarmanu/deeplab-lakeice-webcams).
3. Lake ice detection from Sentinel-1 SAR with deep learning. [Github repo (tensorflow code, pre-trained model)](https://github.com/czarmanu/sentinel_lakeice). [Paper](https://www.isprs-ann-photogramm-remote-sens-spatial-inf-sci.net/V-3-2020/409/2020/) 
4. Tom, M., Wu, T., Baltsavias, E., Schindler, K., 2021. Recent Ice Trends in Swiss Mountain Lakes: 20-year Analysis of MODIS Imagery. [Paper](https://arxiv.org/abs/2103.12434)
5. Tom, M., Jiang, Y., Baltsavias, E., Schindler, K., 2021. Learning a Sensor-invariant Embedding of Satellite Data: A Case Study for Lake Ice Monitoring. [Paper](https://arxiv.org/abs/2107.09092)
6. Tom, M., Suetterlin, M., Bouffard, D., Rothermel, M., Wunderle, S., Baltsavias, E., 2019. [Integrated monitoring of ice
in selected Swiss lakes](https://arxiv.org/abs/2008.00512). Final Project Report
7. Tom, M., Baltsavias, E., Schindler, K., 2020. [Integrated Lake Ice Monitoring and Generation of Sustainable, Reliable, Long Time-Series](https://ethz.ch/content/dam/ethz/special-interest/baug/igp/photogrammetry-remote-sensing-dam/documents/pdf/Misc/Lake_Ice_Project_Final_Report.pdf). Final Project Report


