# VISGA

Seeking Similarities over Differences: 
Similarity-based Domain Alignment for Adaptive Object Detection: [arXiv](https://arxiv.org/pdf/2110.01428.pdf), [Video](https://youtu.be/80nVoFubm3c), [ICCV2021](https://openaccess.thecvf.com/content/ICCV2021/papers/Rezaeianaran_Seeking_Similarities_Over_Differences_Similarity-Based_Domain_Alignment_for_Adaptive_Object_ICCV_2021_paper.pdf)

## Abstract

In order to robustly deploy object detectors across a wide range  of  scenarios,  they  should  be  adaptable  to  shifts  in the  input  distribution  without  the  need  to  constantly  annotate  new  data.   This  has  motivated  research  in  Unsupervised Domain Adaptation (UDA) algorithms for detection.  UDA methods learn to adapt from labeled source domains to unlabeled target domains, by inducing alignment between detector features from source and target domains. Yet, there is no consensus on what features to align and how to do the alignment.  In our work, we propose a framework that  generalizes  the  different  components  commonly  used by UDA methods laying the ground for an in-depth analysis of the UDA design space.  Specifically,  we propose a novel UDA algorithm,  ViSGA, a direct implementation of our framework, that leverages the best design choices and introduces a simple but effective method to aggregate features at instance-level based on visual similarity before inducing group alignment via adversarial training.  We show that both similarity-based grouping and adversarial training allows our model to focus on coarsely aligning feature groups, without being forced to match all instances across loosely aligned domains.  Finally, we examine the applicability of ViSGA to the setting where labeled data are gathered from different sources. Experiments show that not only our method outperforms previous single-source approaches on Sim2Real and Adverse Weather, but also generalizes well to the multi-source setting.

[![ViSGA: Check our video!](https://img.youtube.com/vi/80nVoFubm3c/0.jpg)](https://www.youtube.com/watch?v=80nVoFubm3c "ViSGA: Check our video!")

## Pretrained Model & Results
The following results are all tested with Resnet-50 backbone. By using this implementation "[Domain Adaptive Faster R-CNN in PyTorch](https://github.com/krumo/Domain-Adaptive-Faster-RCNN-PyTorch)", you can test our models. 

| Scenario                       | AP@50 |  url  | im / gpu |  logs  |
|--------------------------------|:-----:|:-----:|:--------:|--------|
| Cityscapes to Foggy Cityscapes | 43.3 |[ model ](https://drive.google.com/file/d/198gifZixYBnJtZoOOCgOwxgJeIHT5FIO/view?usp=sharing)|    2     |  [log](https://drive.google.com/file/d/1xCsh_YkmXSllOl8ZtGfpWRe5_JeHoa6w/view?usp=sharing)  |
| Sim10k to Cityscapes           | 49.3 |[ model ](https://drive.google.com/file/d/19BEVuCysfsY7D4ljw8JUEO5eUa64CVzu/view?usp=sharing)|    2     |  [log](https://drive.google.com/file/d/1znk0pjiLGhW_n-60lenCa6bHCen7m0xc/view?usp=sharing)  |
| Kitti to Cityscapes            | 47.6 |[ model ](https://drive.google.com/file/d/134tLyuY5mNszM4RPijMIr03u3Ng4AX4I/view?usp=sharing)|    2     |  [log](https://drive.google.com/file/d/1m8teK2MJFPa788e9puhTtVInK_HYbVjN/view?usp=sharing)  |
| Multi-source                   | 51.3 |[ model ](https://drive.google.com/file/d/1S0jNCvLEKEZIoLrWA70tT8BKYoWYI6jT/view?usp=sharing)|    2     |  [log](https://drive.google.com/file/d/19HSCbivoumn0dqaIl3yHzHHt4k1fwNwu/view?usp=sharing)  |
