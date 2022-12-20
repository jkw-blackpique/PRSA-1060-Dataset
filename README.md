# PRSA-1060 Dataset

The PRSA-1060 Person Re-identification in Surveillance-Aerial Imagery Dataset.

Our PRSA-1060 is released now！<br>

Thanks for your interest in our PRSA-1060 dataset.<br>

![Overview](https://github.com/jkw-blackpique/PRSA-1060-Dataset/blob/main/Figure1.jpg)

Our PRSA-1060 dataset is used for person re-identification research in surveillance-aerial imagery. With the rapid development of Unmanned Aerial Vehicles (UAVs), UAV-based vision applications have been drawing increasing attention from both industry and academia. However, UAV-based person re-identification is rarely studied, although it has a variety of potential applications such as long-term tracking, visual object retrieval, etc. One of the reasons is the lack of a corresponding publicly available dataset, which will take a large number of human efforts for UAV ﬂying, video capture, and data annotation. And more importantly, there is a huge perspective gap between two common sources of personal data, surveillance imagery and aerial imagery, which will make it hard to combine surveillance imagery and aerial imagery for personal re-identification. In this case, we collect and release our PRSA-1060 to support in-depth research, providing surveillance imagery and aerial imagery with view-angle gaps in several scenes.<br>

Our PRSA-1060 dataset consists of 1,060 identities and 15,753 person bounding boxes captured by nine cameras, seven in HD and two in low HD. Each person is captured by three cameras, two providing surveillance perspective and one providing aerial perspective, and has multiple images under one camera.


## Dataset partition

The current version of the PRSA-1060 dataset only contains testing set that is split to the query set and gallery set, among which the query set contains 4,777 images with 971 IDs, and the gallery set contains 10,976 images with 1,060 IDs. We propose to use the PRSA-1060 dataset in conjunction with other general person re-identification datasets, for example, training on the general datasets and testing on our PRSA-1060 dataset to evaluate the perspective generalization ability of the model. In addition, we will continue to update and support the PRSA-1060 dataset in the future, and propose a larger and diverse version, and the training set will be included.<br>


## Dataset structure

PRSA-1060<br>
　　├── images<br>
　　　　├── 000001_01_001_00003090.jpg<br>
　　　　├── 000001_01_001_00003100.jpg<br>
　　　　├── 000001_01_001_00003120.jpg<br>
　　　　├── ......<br>
　　├── partitions.pkl<br>
　　└── README.md<br>

images: The 15,753 person bounding boxes of our PRSA-1060 dataset.<br>
partitions.pkl: The file describing the partitioning of our PRSA-1060 dataset.<br>
README.md: Just this file.<br>


## Annotation

Image name: PersonID_CameraID_VideoID_Frame.jpg, such as 00000X_0Y_00Z_0000000A.jpg, the 00000X indicates this image belongs to Person ID No.X, the 0Y indicates this image is captured by camera No.Y, 00Z indicates this image is extracted from video No.Z under this camera and 0000000A indicates this image is the Z-th frame in this video.

        
## Evaluation Metrics

We adopt the popular mean Average Precision (mAP) and Cumulative Matching Cure (CMC) as in other re-identification works.


## Downloading

You can get the downloading link of our PRSA-1060 dataset via sending e-mail to us.

Our e-mail address: <jkw-blackpique@outlook.com>


## Statement

Our PRSA-1060 dataset is prohibited for any commercial using. If you use PRSA-1060 dataset in your research, you should refer to our work as the following BibTeX entry.

```
@misc{PRSA-1060,
  author = {jkw-blackpique},
  title = {PRSA-1060 Dataset},
  year = {2022},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {<https://github.com/jkw-blackpique/PRSA-1060-Dataset>}
}
```


