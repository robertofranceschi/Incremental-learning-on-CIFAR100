# Class-Incremental Learning in Image Recognition

##### Roberto Franceschi, Gabriele Tiboni, Alessandro Desole

![image](https://user-images.githubusercontent.com/57017982/205986525-de2f7f40-7313-4366-b355-731970cfd23c.png)

### Abstract

<p align="justify">
Recent studies in machine learning aim at developing models that are able to incrementally learn new concepts over time with minimal effort in terms of resource usage. In this work, we recall and reproduce from scratch two of the most popular approaches to this problem (”Learning without forgetting” and ”iCaRL”) and we conduct an in-depth ablation study on the previous methods. We finally propose a variation that exploits an implicit hysteresis effect of the network when storing a dynamic number of samples from old classes throughout the incremental learning process, which allows to consistently increase the average performances without varying the overall resource overhead.
</p>

---

### Resources:

- [Report (pdf)](./Final%20Report.pdf)
- [Experiments and Results (spreadsheet)](https://docs.google.com/spreadsheets/d/1lxrz5nrHcYjzODCsvCoGal30N-beyxo3r65X9YPig6E/edit?usp=sharing)
- Code is made available directly in colab at the following links.
  
  | Model | Description | Notebook |
  | --- | --- | --- |
  | Finetuning and JointTraining | Baseline models illustrating traditional approaches with their inherent limitations such as catastrophic forgetting. | [Open In Colab](https://drive.google.com/file/d/1cDOSFWes1lKWipprQMQn2ww-emaUAZ_m/view?usp=share_link) |
  | Learning without Forgetting | Utilizes knowledge distillation to preserve performance on previous tasks while learning new ones, minimizing forgetting. | [Open In Colab](https://drive.google.com/file/d/1wjK0EK4828dyICHwVtZ6Ob-0eML9qNa1/view?usp=share_link) |
  | iCaRL | Combines representation learning with class exemplar retention to effectively manage class incremental learning. | [Open In Colab](https://drive.google.com/file/d/1HmShDAiKIU0wroo7NyAWfkGqK5ck36qh/view?usp=share_link) |
  | Ablation Experiments (Losses) | Explores the impact of different loss functions on the balance between retaining old knowledge and acquiring new information. | [Open In Colab](https://drive.google.com/file/d/1Kdl6HPOZAZrBTim1ETwIHrxR3-f_VLjx/view?usp=share_link) |
  | Our Proposal | Introduces a dynamic exemplar management strategy, enhancing model adaptability and performance in an incremental learning setting. | [Open In Colab](https://drive.google.com/file/d/1N1mO7_LSirTDdhzB3Xpme6_6MK95gO9A/view?usp=share_link) |

---

#### References

[1] Abien Fred Agarap. Deep learning using rectified linear units (relu). ArXiv, abs/1803.08375, 2018.

[2] Rich Caruana. Multitask learning. Mach. Learn., 28(1):41–75, July 1997.

[3] Ross B. Girshick, Jeff Donahue, Trevor Darrell, and Jagannath Malik. Rich feature hierarchies for accurate object detection and semantic segmentation. 2014 IEEE Conference on Computer Vision and Pattern Recognition, pages 580–587, 2014.

[4] Ian J. Goodfellow, Mehdi Mirza, Xia Da, Aaron C. Courville, and Yoshua Bengio. An empirical investigation of catastrophic forgetting in gradient-based neural networks. CoRR, abs/1312.6211, 2014.

[5] Kaiming He, Xiangyu Zhang, Shaoqing Ren, and Jian Sun. Deep residual learning for image recognition. CoRR, abs/1512.03385, 2015.

[6] Kaiming He, Xiangyu Zhang, Shaoqing Ren, and Jian Sun. Delving deep into rectifiers: Surpassing human-level performance on imagenet classification. 2015 IEEE International Conference on Computer Vision (ICCV), pages 1026–1034, 2015.

[7] Geoffrey E. Hinton, Oriol Vinyals, and Jeffrey Dean. Distilling the knowledge in a neural network. ArXiv, abs/1503.02531, 2015.

[8] Saihui Hou, Xinyu Pan, Chen Change Loy, Zilei Wang, and Dahua Lin. Learning a unified classifier incrementally via rebalancing. June 2019.

[9] Alex Krizhevsky. Learning multiple layers of features from tiny images. University of Toronto, 05 2012.

[10] Zhizhong Li and Derek Hoiem. Learning without forgetting. CoRR, abs/1606.09282, 2016.

[11] Chunjie Luo, Jianfeng Zhan, Lei Wang, and Qiang Yang. Cosine normalization: Using cosine similarity instead of dot product in neural networks. CoRR, abs/1702.05870, 2017. 15

[12] Michael McCloskey and Neal J. Cohen. Catastrophic interference in connectionist networks: The sequential learning problem. Psychology of Learning and Motivation, 24:109–165, 1989.

[13] Sylvestre-Alvise Rebuffi, Alexander Kolesnikov, and Christoph H. Lampert. icarl: Incremental classifier and representation learning. CoRR, abs/1611.07725, 2016.
