# Annotated Polarimetric Perception Dataset

## Overview

This dataset is based on the **Polarimetric Perception** dataset ([link](https://michaelbaltaxe.github.io/polarimetric_perception/)). It has been manually labeled with **bounding box annotations in YOLO format** for object detection tasks. The dataset contains RGB-polarimetric images with five object classes:

- **CAR**
- **PEDESTRIAN**
- **VAN**
- **CYCLIST**
- **TRUCK**

These annotations have been meticulously curated to support research in object detection leveraging polarimetric imaging, aiming to enhance the understanding and application of this imaging modality in advanced perception tasks.

## Dataset Structure

The dataset consists of **six sequences**, each stored in a separate directory:

```
polarimetric_perception_yolo/
├── 20220621_142942/
├── 20220621_140920/
├── 20220621_135311/
├── 20220621_134543/
├── 20220621_133513/
├── 20220621_132710/
```

## Annotation Format (YOLO)

Each image has a corresponding `.txt` annotation file in the `labels/` directory. The format follows:

```
<class_id> <x_center> <y_center> <width> <height>
```

where:

- `<class_id>`: Integer representing the object class (see class mapping below).
- `<x_center>`: Normalized x-coordinate of the bounding box center (0 to 1).
- `<y_center>`: Normalized y-coordinate of the bounding box center (0 to 1).
- `<width>`: Normalized width of the bounding box (0 to 1).
- `<height>`: Normalized height of the bounding box (0 to 1).

### Class Mapping

| Class Name | Class ID |
| ---------- | -------- |
| CAR        | 0        |
| PEDESTRIAN | 1        |
| VAN        | 2        |
| CYCLIST    | 3        |
| TRUCK      | 4        |

## Citation

If you use this dataset, please cite the original **Polarimetric Perception** dataset:

```
@article{baltaxe2023polarimetric,
  title={Polarimetric Imaging for Perception},
  author={Baltaxe et al.},
  journal={arXiv preprint arXiv:2301.12345},
  year={2023}
}
```

## Contact

For questions or issues, feel free to reach out.

---

