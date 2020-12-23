---
title: Data
---
&larr; [Homepage](https://vios-s.github.io/multiscale-adversarial-attention-gates)

## Download

You can download the scribble annotations at [this link](https://github.com/gvalvano/multiscale-adversarial-attention-gates/raw/master/DATA/acdc_scribbles.zip).
File names are the same as in the ACDC dataset. For example, for patient 12 we have the files `patient012_frame_ED_scribble.nii.gz` and `patient012_frame_ES_scribble.nii.gz` for the end-diastolic and end-systolic cardiac phases. 

If you use this data, you should cite our paper as:
```
@article{valvano2020weakly,
  title={Weakly Supervised Segmentation with Multi-scale Adversarial Attention Gates},
  author={Valvano, Gabriele and Leo, Andrea and Tsaftaris, Sotirios A},
  journal={arXiv preprint arXiv:2007.01152},
  year={2020}
}
```

## Data Description

###  ACDC
The 2017 Automatic Cardiac Diagnosis Challenge dataset [1] contains cine-MR images obtained by 100 patients with different MR scanners and acquisition protocols. 
Manual segmentations are provided along with the images, containing pixel-wise annotations for the end-diastolic (ED) and end-systolic (ES) cardiac phases. 
The annotated structures are left ventricle (LV), right ventricle (RV) and myocardium (MYO). 
You can download the data [here](https://www.creatis.insa-lyon.fr/Challenge/acdc/index.html).

### Scribble Generation

To annotate the images with scribbles we used [ITK-SNAP](http://www.itksnap.org/pmwiki/pmwiki.php) [2]. 
We manually drew scribbles for RV, MYO, LV on top of the available segmentation masks provided in ACDC, for ES and ED phases. 
We additionally drew a scribble approximately around the heart to identify pixels belonging to the background class (BGD), while leaving the rest of the pixels 
unlabeled.  The average (standard deviation) image coverage of scribbles is:  0.1 (0.1)%, 0.2 (0.1)%, 0.1 (0.1)% and 10.4 (8.4)%, 
for RV, MYO, LV and BGD, respectively.

### Reference
[1] *O. Bernard, A. Lalande, C. Zotti, F. Cervenansky, X. Yang, P.-A. Heng, I. Cetin, K. Lekadir, O. Camara, M. A. G. Ballester et al., 
“Deep learning techniques for automatic MRI cardiac multi-structures segmentation and diagnosis: Is the problem solved?” 
IEEE TMI, vol. 37, no. 11, pp. 2514– 2525, 2018.*

[2] *P. A. Yushkevich, J. Piven, H. Cody Hazlett, R. Gimpel Smith, S. Ho, J. C. Gee, and G. Gerig, 
“User-Guided 3D Active Contour Segmentation of Anatomical Structures: Significantly Improved Efficiency and Reliability” 
Neuroimage, vol. 31, no. 3, pp. 1116–1128, 2006.*

## Don't miss any update!
**You can either:**
 - **fill out** [**this form**](https://docs.google.com/forms/d/e/1FAIpQLSdXVFqMuc3Q_ojNkYWBkDNLd8sBNGjVkHw4oLx2xgZbN2EWXg/viewform?usp=sf_link), and we will contact you with updates on *code* and *data*
 - or **write us an** [**email**](https://gvalvano.github.io/wss-multiscale-adversarial-attention-gates/contacts), and we will answer back
 - or **watch the** [**GitHub**](https://github.com/gvalvano/multiscale-adversarial-attention-gates) repository for updates on the *code*
