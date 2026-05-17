# Daily-Interference-Pressure-Dataset
The public dataset called Daily Interference Pressure Dataset is used for pressure-based in-bed pose estimation researches under daily interference.

This repository accompanies the paper:

**Pressure distribution based 2D in-bed keypoint prediction under interfered scenes**

## Dataset Overview

The dataset contains:

- 2472 synchronized RGB-D and pressure frames 
- 10 subjects
- 8 scenarios simulating home settings
- 4 types interference object
- Pixel-level annotation about interference
- 2D joint position annotation

Raw data can be found in the **original_data** folder. Because of the limitation, the RGB images and depth images are unable to be uploaded in this repository, please contact [kyrickie@mail.ustc.edu.cn](mailto:kyrickie@mail.ustc.edu.cn) if you need.

Processed data can be found in the [DIP.h5](DIP.h5) file.

[unseen_objects.h5](unseen_objects.h5) is a test set containing different interference objects.

The keys in the h5 files are as follows:

- **data_pure**: raw pressure image data.
- **interference_predict**: predicted interference mask, middle-productions using the method introduced in the paper
- **label_auto**: pixel-level annotation about interference mask
- **pck_th**: PCK threshold used in the paper
- **person**: subject's ID
- **pos**: posture's ID
- **ps_joint**: 2D joint position annotation
- **scene**: scenario's ID

## Ethical Approval

This study was performed in line with the principles of the Declaration of Helsinki.

Ethical approval was granted by the **Medical Research Ethics Committee of The First Affiliated Hospital of the University of Science and Technology of China (USTC)**.

Approval No.: **2023KY-441**

## Citation

The formal citation will be added after publication.

If you use the DIP dataset, please cite the paper:

```text
Ke Y, Wan Q, Xie F, et al. Pressure distribution based 2D in-bed keypoint prediction under interfered scenes[J]. Pervasive and Mobile Computing, 2024, 105: 101979.
```

## Contact

For dataset access, questions, or reporting potential privacy/security concerns, please contact:

**Yi Ke**  
Email: [kyrickie@mail.ustc.edu.cn](mailto:kyrickie@mail.ustc.edu.cn)
