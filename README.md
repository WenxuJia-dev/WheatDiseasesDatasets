# Wheat YOLO dataset

This repository contains the Wheat_YOLO image and annotation files supplied for the ERNR-YOLO study. The files are distributed in five ZIP archives, tracked with Git LFS. Download all five archives and extract each one into the same directory to reconstruct the original folder structure:

```
images/train_new/
images/val/
labels/train_new/
labels/val/
```

Each image has a corresponding YOLO-format text annotation with the same filename stem. The supplied data contain 11,459 training images and 2,828 images in the `val` directory, with 26,495 bounding-box annotations in total. A separate test folder and class-name mapping were not present in the supplied directory; the `val` directory is published as provided, without assuming a validation/test subdivision.

A byte-level check found 15 duplicate occurrences across the supplied training and `val` folders. Researchers should account for this overlap when designing evaluation splits. The archives preserve the supplied files without modification.

Files are distributed via Git LFS. To download them using Git, install Git LFS and run `git lfs install` before cloning. The SHA-256 checksums are listed in `SHA256SUMS`.
