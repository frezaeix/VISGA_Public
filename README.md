# VISGA

Seeking Similarities over Differences: 
Similarity-based Domain Alignment for Adaptive Object Detection: [arXiv](https://arxiv.org/pdf/2110.01428.pdf), [Video](https://youtu.be/80nVoFubm3c), [ICCV2021](https://openaccess.thecvf.com/content/ICCV2021/papers/Rezaeianaran_Seeking_Similarities_Over_Differences_Similarity-Based_Domain_Alignment_for_Adaptive_Object_ICCV_2021_paper.pdf)

## Abstract

In order to robustly deploy object detectors across a wide range  of  scenarios,  they  should  be  adaptable  to  shifts  in the  input  distribution  without  the  need  to  constantly  annotate  new  data.   This  has  motivated  research  in  Unsupervised Domain Adaptation (UDA) algorithms for detection.  UDA methods learn to adapt from labeled source domains to unlabeled target domains, by inducing alignment between detector features from source and target domains. Yet, there is no consensus on what features to align and how to do the alignment.  In our work, we propose a framework that  generalizes  the  different  components  commonly  used by UDA methods laying the ground for an in-depth analysis of the UDA design space.  Specifically,  we propose a novel UDA algorithm,  ViSGA, a direct implementation ofour framework, that leverages the best design choices andintroduces a simple but effective method to aggregate fea-tures at instance-level based on visual similarity before inducing group alignment via adversarial training.  We show that both similarity-based grouping and adversarial training allows our model to focus on coarsely aligning feature groups, without being forced to match all instances across loosely aligned domains.  Finally, we examine the applicability of ViSGA to the setting where labeled data are gathered from different sources. Experiments show that not only our method outperforms previous single-source approaches on Sim2Real and Adverse Weather, but also generalizes well to the multi-source setting.

[![ViSGA: Check our video!](https://img.youtube.com/vi/80nVoFubm3c/0.jpg)](https://www.youtube.com/watch?v=80nVoFubm3c "ViSGA: Check our video!")
