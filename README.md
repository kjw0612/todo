# Doing
- Comparing Image Patches. This idea can be applied to both SR and Deblur and more. 
  - Learning to Compare Image Patches via Convolutional Neural Networks, CVPR 2015 http://imagine.enpc.fr/~zagoruys/deepcompare.html   
- Studying various learning techniques - domain adaptation, one shot zero shot 
  - Domain-Adversarial Training of Neural Networks
- Content-aware prior http://people.csail.mit.edu/taegsang/Documents/ContentAwarePrior_CVPR2010.pdf
- ICLR 2015 cohen and welling http://arxiv.org/pdf/1412.7659v3.pdf

# Assigns

- Jonghyuk : JPEG Artifact removal 8/18
- Jung Kwon : Restoration Framework 

# Todo
# Idea
## Image Restoration
- Total Restoration 
- Multi-Task Learning: priors shared between tasks. generalizing better to new tasks. 36p. of dlss-3aug2015.pdf (Bengio DLSS 2015)
- Use results from semantic, object recognition, edge detection to do better sr

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

- ICLR Presentations with Video https://www.youtube.com/channel/UCqxFGrNL5nX10lS62bswp9w

# Read 

- http://arxiv.org/pdf/1411.2539.pdf
- http://papers.nips.cc/paper/5422-on-the-number-of-linear-regions-of-deep-neural-networks.pdf
- Adam: http://arxiv.org/pdf/1412.6980v8.pdf
- Generative modeling
  - VAE:Variational Autoencoder (Kingma et al., 2014), 85 cites
  - DARN: Deep Autoregressive Networks (Gregor et al. 2014), 35 
  - DRAW:DeepRecurrentAttentiveWriter(Gregoretal.2015), 18
  - GAN: Generative Adversarial Networks (Goodfellow et al. 2014), 21 
  - GSN: Generative Stochastic Networks (Bengio et al. 2014), 66
  - DBM: deep Boltzmann machines (Salakhutdinov and Hinton, 2009), 456
  - Deep Generative Image Models using a Laplacian Pyramid of Adversarial Networks, Fergus. 
  
## NIPS 2015
- faster R cNN http://arxiv.org/pdf/1506.01497v1.pdf
- Perceiving Physical Object Properties by Integrating a Physics Engine with Deep Learning
Jiajun Wu*, MIT; Ilker Yildirim, MIT; William Freeman, MIT; Josh Tenenbaum, MIT
- Expressing an Image Stream with a Sequence of Natural Sentences
Cesc Park, Seoul National University; Gunhee Kim*, Seoul National University
- Inferring Algorithmic Patterns with Stack-Augmented Recurrent Nets
Armand Joulin*, Facebook AI research; Tomas Mikolov, Facebook AI Research
- Where are they looking?
Adria Recasens*, MIT; Aditya Khosla, MIT; Carl Vondrick, MIT; Antonio Torralba, MIT
- Bidirectional Recurrent Convolutional Networks for Multi-Frame Super-Resolution
Yan Huang*, CRIPAC, CASIA; Wei Wang, NLPR,CASIA; Liang Wang, 
- Texture synthesis and the controlled generation of natural stimuli using convolutional neural networks
Leon Gatys*, University of Tübingen; Alexander Ecker, University of Tuebingen; Matthias Bethge, CIN, University Tübingen
- Learning visual biases from human imagination
Carl Vondrick*, MIT; Hamed Pirsiavash, MIT; Aude Oliva, MIT; Antonio Torralba, MIT
- Deeply Learning the Messages in Message Passing Inference
Guosheng Lin*, The University of Adelaide; Chunhua Shen, ; Ian Reid, University of Adelaide; Anton Van Den Hengel, University of Adelaide
- 3D Object Proposals for Accurate Object Class Detection
Xiaozhi Chen, Tsinghua University; Kaustav Kundu, University of Toronto; Yukun Zhu, University of Toronto; Andrew Berneshawi, University of Toronto; Huimin Ma, Tsinghua University; Sanja Fidler, University of Toronto; Raquel Urtasun*, University of Toronto
- Tensorizing Neural Networks
Alexander Novikov*, Skolkovo institute of science ; Dmitry Podoprihin, msu; Anton Osokin, Inria; Dmitry Vetrov, 
- Attention-Based Models for Speech Recognition
Jan Chorowski*, University of Wroclaw; Dzmitry Bahdanau, Jacobs University, Germany; Dmitriy Serdyuk, Université de Montréal; Kyunghyun Cho, NYU; Yoshua Bengio, U. Montreal
- Character-level Convolutional Networks for Text Classification
Xiang Zhang*, New York University; Junbo Zhao, New York University; Yann LeCun, New York University
- Deep learning with Elastic Averaging SGD
Sixin Zhang*, New York University; Anna Choromanska, Courant Institute, NYU; Yann LeCun, New York University
- Shepard Convolutional Neural Networks
Jimmy Ren*, SenseTime Group Limited; Li Xu, SenseTime Group Limited; Qiong Yan, SenseTime Group Limited; Wenxiu Sun, SenseTime Group Limited
- Convolutional Neural Networks with Intra-Layer Recurrent Connections for Scene Labeling
Ming Liang, Tsinghua University; Xiaolin Hu*, Tsinghua University; Bo Zhang, Tsinghua University
- Unsupervised Learning by Program Synthesis
Kevin Ellis*, MIT; Josh Tenenbaum, MIT; Armando Solar-Lezama, MIT
- Learning to Rotate 3D Objects with Recurrent Convolutional Encoder-Decoder Networks
Jimei Yang*, UC Merced; Scott Reed, University of Michigan; Ming-Hsuan Yang, UC Merced; Honglak Lee, U. Michigan
- Deep Visual Analogy-Making
Scott Reed*, University of Michigan; Yi Zhang, University of Michigan; Yuting Zhang, University of Michigan; Honglak Lee, U. Michigan
- Teaching Machines to Read and Comprehend
Karl Moritz Hermann*, Google DeepMind; Tomas Kocisky, Oxford University; Edward Grefenstette, Google DeepMind; Lasse Espeholt, Google DeepMind; Will Kay, Google DeepMind; Mustafa Suleyman, Google DeepMind; Phil Blunsom, Google DeepMind
- Efficient Non-greedy Optimization of Decision Trees and Forests
Mohammad Norouzi, University of Toronto; Maxwell Collins*, UW-Madison; Matthew Johnson, Microsoft Research; David Fleet, University of Toronto; Pushmeet Kohli, Microsoft Research
- Max-Margin Deep Generative Models
Chongxuan Li*, Tsinghua University; Jun Zhu, Tsinghua University; Tianlin Shi, Tsinghua University; Bo Zhang, Tsinghua University
- Generative Image Modeling Using Spatial LSTMs
Lucas Theis*, U.Tuebingen; Matthias Bethge, CIN, University Tübingen
- Learning to Segment Object Candidates
Pedro Pinheiro*, EPFL; Ronan Collobert, Facebook; Piotr Dollar, Facebook AI Research
- Spatial Transformer Networks
Max Jaderberg*, Google; Karen Simonyan, Google DeepMind; Andrew Zisserman, Google; Koray Kavukcuoglu, Google DeepMind
- Learning with a Wasserstein Loss
Chiyuan Zhang*, MIT; Charlie Frogner, MIT; Hossein Mobahi, MIT; Mauricio Araya, Shell Intl. E&P Inc.; Tomaso Poggio, MIT
- Natural Neural Networks
Guillaume Desjardins*, Google DeepMind; Karen Simonyan, Google DeepMind; Razvan Pascanu, Google DeepMind; Koray Kavukcuoglu, Google DeepMind
- Training Very Deep Networks
Rupesh Srivastava*, IDSIA; Klaus Greff, IDSIA; J?rgen Schmidhuber, 
- End-To-End Memory Networks
Sainbayar Sukhbaatar*, New York University; Arthur Szlam, Facebook; Jason Weston, Facebook AI Research; Rob Fergus, Facebook AI Research
- Deep Convolutional Inverse Graphics Network
Pushmeet Kohli, Microsoft Research; Will Whitney, MIT; Tejas Kulkarni*, MIT; Josh Tenenbaum, MIT
- Learning Wake-Sleep Recurrent Attention Models
Jimmy Ba*, University of Toronto; Ruslan Salakhutdinov, University of Toronto; Roger Grosse, University of Toronto; Brendan Frey, U. Toronto
- Neural Adaptive Sequential Monte Carlo
Shane Gu*, ; Richard Turner, neuroscience; Zoubin Ghahramani, University of Cambridge
- Super-Resolution Off the Grid
Qingqing Huang, MIT; Sham Kakade*, University of Washington
- The Return of the Gating Network: combining generative models and discriminative training in natural image priors.
Dan Rosenbaum*, The Hebrew University; Yair Weiss, Hebrew University
- Pointer Networks
Oriol Vinyals*, Google; Meire Fortunato, ; Navdeep Jaitly, Google
- Grammar as a Foreign Language
Oriol Vinyals*, Google; Lukasz Kaiser, Google; Terry Koo, Google; Slav Petrov, Google; Ilya Sutskever, Google; Geoffrey Hinton, Google
- 




  
# Questions

- Can I convert nb into CVPR-formatted PDF directly?

## Courses

- Stanford CS224d
- Stanford CS231n

## Misc.
- https://www.youtube.com/watch?v=OcFOWIq3cIc

# AIKorea
## Ideas
- Record and explain popular posts (or translate) 
