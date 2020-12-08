# SeeingThroughFog_ImageOnly

The SSD300 Halfway Fusion is based on https://github.com/pierluigiferrari/ssd_keras work and is thought to be used with the images from the DENSE datased (link to the paper https://www.cs.princeton.edu/~fheide/AdverseWeatherFusion/figures/AdverseWeatherFusion.pdf), specifically, the RGB (/cam_stereo_left_lut) and the NIR (triple merge of /gated0_rect8, /gated1_rect8 and /gated2_rect8).
@InProceedings{Bijelic_2020_STF,
    author={Bijelic, Mario and Gruber, Tobias and Mannan, Fahim and Kraus, Florian and Ritter, Werner and Dietmayer, Klaus and Heide, Felix},
    title={Seeing Through Fog Without Seeing Fog:
    Deep Multimodal Sensor Fusion in Unseen Adverse Weather},
    booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
    month = {June},
    year = {2020}
}

To download the images please register first using the following link: https://www.uni-ulm.de/en/in/driveu/projects/dense-datasets/dense-registration-form/

The SSD300 model expects two inputs of images with shape (300,300,3), a previous homography conversion should be applied to match pixel-wise the RGB and NIR images.
