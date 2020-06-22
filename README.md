# Notice: This repository is deprecated, please use https://github.com/calmevtime/DCTNet.

# Learning in the Frequency Domain


This is the source code for the CVPR'20 paper entitled "Learning in the Frequency Domain" (https://arxiv.org/abs/2002.12416).

## Highlights
* We propose a method of learning in the frequency domain (using DCT coefficients as input), which requires little modification to the existing CNN models that take RGB input. We validate our method on ResNet50 and MobileNetV2 for the image classification task and Mask R-CNN for the instance segmentation task.
* We show that learning in the frequency domain better preserves image information in the pre-processing stage than the conventional spatial downsampling approach (spatially resizing the images to 224×224, the default input size of most CNN models) and consequently achieves improved accuracy, i.e., +1.41% on ResNet-50 and +0.66% on MobileNetV2 for the ImageNet classification task, +0.8% on Mask R-CNN for both object detection and instance segmentation tasks.
* We analyze the spectral bias from the frequency perspective and show that the CNN models are more sensitive to low-frequency channels than high-frequency channels, similar to the human visual system (HVS).
* We propose a learning-based dynamic channel selection method to identify the trivial frequency components for static removal during inference. Experiment results on ResNet-50 show that one can prune up to 87.5% of the frequency channels using the proposed channel selection method with no or little accuracy degradation in the ImageNet classification task.
* To the best of our knowledge, this is the first work that explores learning in the frequency domain for object detection and instance segmentation. Experiment results on Mask R-CNN show that learning in the frequency domain can achieve a 0.8% average precision improvement for the instance segmentation task on the COCO dataset.

Please refer to the [image classfication](classification) and [instance segmentation](segmentation) sections for more details.

Note: This a cloned repo of https://github.com/calmevtime/DCTNet.
