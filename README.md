# Doing
- DLSS 2015 Study All Day 2 (Hugo First One Done)
- Studying various learning techniques - domain adaptation, one shot zero shot 
  - Domain-Adversarial Training of Neural Networks

# Assigns

- Jonghyuk : JPEG Artifact removal 8/18
- Jung Kwon : Restoration Framework 

# Todo
# Idea
## Image Restoration
- Total Restoration 
- Multi-Task Learning: priors shared between tasks. generalizing better to new tasks. 36p. of dlss-3aug2015.pdf (Bengio DLSS 2015)

### Single-Image Super-Resolution
- Progressive SR

### Video Super-Resolution

### Deblurring
- End-to-end deblur (without finding a kernel)
- Generative model. Capture the same scence twice (clean/blur). View it as a classfication problem (same scene positive, different scene negative). as in stereo cnn, first input image clean second blur. After several CNNs for each stream, they get concatenated and classification is done. After this, generative model is explored. When blur image and class (same scene, positive) are given, clean image is sampled. I need study for generative model for these stuffs.

## Semantic Segmentation

- Low-level network (SR, Noise Reduction) -> Higher-level network (Semantic Seg.)
- CNN for baseline prediction. RNN (visual-attention model) wanders around to collect contextual evidence

## Stereo
- Super-Resolution and then Stereo (replace phase-shift in http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Jeon_Accurate_Depth_Map_2015_CVPR_paper.pdf)

# Study

# Read 

- http://papers.nips.cc/paper/5422-on-the-number-of-linear-regions-of-deep-neural-networks.pdf
- Adam: http://arxiv.org/pdf/1412.6980v8.pdf

# Questions

- Can I convert nb into CVPR-formatted PDF directly?

## Courses

- Stanford CS224d
- Stanford CS231n
