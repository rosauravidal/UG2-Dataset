# UG<sup>2</sup> Dataset
> A Video Benchmark for Assessing the Impact of Image Restoration and Enhancement on Automatic Visual Recognition

The UG<sup>2</sup> Dataset (UAV, Glider, and Ground) contains manually annotated videos from challenging imaging scenarios containing mobile airborne cameras (**UAV, Gliders**) and **Ground**-based captures. While we provide frame-level annotations for the purpose of object classification, the annotations can be re-purposed for other high-level tasks such as object detection and tracking

## Download

[Google Drive](https://goo.gl/AjA6En)

## Citation
If you use this dataset in your research, please cite our work as:

```
@inproceedings{vidal2018ug,
  title={Ug\^{} 2: A video benchmark for assessing the impact of image restoration and enhancement on automatic visual recognition},
  author={Vidal, Rosaura G and Banerjee, Sreya and Grm, Klemen and Struc, Vitomir and Scheirer, Walter J},
  booktitle={2018 IEEE Winter Conference on Applications of Computer Vision (WACV)},
  pages={1597--1606},
  year={2018},
  organization={IEEE}
}
```

## Dataset stats

### Training partition
The training dataset is composed of 629 videos with 3,535,382 frames, representing 228 ImageNet classes extracted from annotated frames from the three different video collections. These classes are further categorized into 37 super-classes encompassing visually similar ImageNet categories and two additional classes for pedestrian and resolution chart images. 


Collection | UAV | Glider | Ground | Total
---------- | --- | ------ | ------ | -----
Total Videos | 231 | 120 | 278 | 629
Total Frames | 1,501,675 | 1,840,160 | 193,547 | 3,535,382 
Annotated Videos | 30 | 30 | 136 | 196
Annotated Frames | 28,263 | 25,246 | 98,574 | 152,083 
Extracted Objects | 29,826 | 31,760 | 98,574 | 160,160
Object Classes | 31 | 20 | 20 | 37 

The dataset contains a subset of 152,083 object-level annotated frames where 160,160 objects are fully visible (out of 200,694 total annotated frames) and the videos are tagged to indicate problematic conditions.

Over 70% of the UG<sup>2</sup> classes have more than 400 images and 58% of the classes are present in the imagery of at least two collections. Around 20% of the classes are present in all three collections.  

### Testing partition

The testing dataset is composed of 55 videos with frame-level annotations. Out of the annotated frames, 8,910 disjoint frames were selected among the three different video collections, from which we extracted 9,187 objects. These objects are further categorized into 42 super-classes encompassing visually similar ImageNet categories. While most of the super-classes in the testing dataset overlap with those in the training dataset, there are some classes unique to each.

Collection | UAV | Glider | Ground | Total
---------- | --- | ------ | ------ | -----
Total Videos | 19 | 15 | 21 | 55 
Annotated Frames | 2,814 | 2,909 | 3,187 | 8,910  
Extracted Objects | 3,000 | 3,000 | 3,187 | 9,187
Object-Classes | 28 | 17 | 20 | 42

## Annotation format

Bounding boxes establishing object regions were manually annotated using the [VATIC Video Annotation Tool](https://github.com/cvondrick/vatic/tree/contrib). We provide the VATIC annotation files for every annotated video in the dataset.
