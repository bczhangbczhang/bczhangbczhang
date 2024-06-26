I am a professor at one of the top universities in China, Beihang University, and Zhongguancun National Laboratory. I am an adjunct professor at the University at Buffalo, and serves as an academic advisor at Baidu's Deep Learning Laboratory. My research focuses on steerable representation for efficient object recognition, and the main research topics include:

1. Gabor Steerable Pattern Features and Gabor CNNs. 

Why visual perception of human being is so efficient and accurate, which kind of mathematical modeling is available to describe this? This is a fundamental issue in the field of computer vision. To answer this question, we introduce a controllable visual representation model, attempting to enable machines to efficiently extract visual features like humans. In the middle of the last century, Nobel laureate Dennis Gabor proposed the Short Time Fourier Transform. Following the idea, Gabor wavelets based on Gaussian windows can achieve a uncertainty minimization. From a more fundamental perspective, Gaussian windows is the most energy-efficient way to perceive the world. This is one of the most successful mathematical modeling works for visual perception and has become a milestone in the field of vision. However, in the process of perceiving things, different positions should have different scales of Gaussian kernels, which intuitively indicates that the mixed Gaussian model is better at modeling human visual perception. However, this requires a theoretical proof of uncertainty boundedness, that is, the model should be still energy-efficient and conforms to the laws of biological evolution. In 2016, I proved the boundedness of uncertainty in target perception systems based on mixed Gaussian wave functions, and innovatively proposed a proof method for scale intervals (IJCV). The smaller the proof interval, the smaller the uncertainty, which made a general extension of Gaussian uncertainty theory.

In this topic, we struggle for many years to understand how Gabor can help us understand computer vision principles. Two “Test-of-Time” papers (first author) on feature extraction based on Gabor wavelets, HGPP and LDP, are highly cited for1282 and 768 times. The HGPP paper, as one of the representative papers contribute to the second prize of the National Natural Science Award. LDP was integrated into a MATLAB scene/object recognition toolkit (denseMBLDP(I, options) shown in examples as demo_denseMBLDP), included in Central File Exchange (Scenes recognition toolbox for vision systems) with more than 13k downloads. Following the path of Gabor-based feature represenation, we develop Gabor CNNs (2018 hot-spot article with 372 Google scholar citations) to improve the performance and interpretability of deep learning models. Our model can produce scale/regional adaptive features based on Gabor modulation and pooling operation. We also provide the  proof and theoretical foundation that the uncertainty of Gaussian mixture models are bounded (first author paper in IJCV 2016). The related work has been published in IJCV/ IEEE TIP/CVPR/TNNLS. The selected papers for this topic are listed as below.

[1] Zhang Baochang, Perina Alessandro, Li Zhigang, Murino Vittorio, Liu Jianzhuang, Ji Rongrong. Bounding multiple gaussians uncertainty with application to object tracking[J]. International journal of computer vision, 2016, 118: 364-379.

[2] Luan Shangzhen, Chen Chen, Zhang Baochang*, Han Jungong*, Liu Jianzhuang. Gabor convolutional networks[J]. IEEE Transactions on Image Processing, 2018, 27(9): 4357-4366.

[3] Wang Runqi, Duan Xiaoyue, Kang Guoliang, Liu Jianzhuang, Lin Shaohui, Xu Songcen, Lu Jinhu, Zhang Baochang*. AttriCLIP: A Non-Incremental Learner for Incremental Knowledge Learning[C]//Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2023 

[4] Zhang Baochang, Wang Runqi, Wang Xiaodi, Han Jungong, Ji Rongrong. Modulated convolutional networks[J]. IEEE Transactions on Neural Networks and Learning Systems, 2021.

[5] Mao Mingyuan , Zhang Renrui , Zheng Honghui , Gao Peng , Ma Teli , Peng Yan , Ding Eerui , Zhang Baochang*, Han Shumin*. Dual-stream network for visual recognition. Advances in Neural Information Processing Systems, 2021, 34: 25346-25358. 

[6] Zhang Baochang, Yang Wankou, Wang Ze, Zhuo Lian, Han Jungong, Zhen Xiantong. The structure transfer machine theory and applications[J]. IEEE Transactions on Image Processing, 2019, 29: 2889-2902.

[7] Baochang Zhang, Shiguang Shan, Xilin Chen, Wen Gao: Histogram of Gabor Phase Patterns (HGPP): A Novel Object Representation Approach for Face Recognition. IEEE Trans. Image Process. 16(1): 57-68 (2007)

[8] Baochang Zhang, Yongsheng Gao, Sanqiang Zhao, Jianzhuang Liu: Local Derivative Pattern Versus Local Binary Pattern: Face Recognition With High-Order Local Pattern Descriptor. IEEE Trans. Image Process. 19(2): 533-544 (2010)

The source code about Gabor CNNs can refer to my student github: https://github.com/jxgu1016

The source code of denseMBLDP(I, options) is shown in examples as demo_denseMBLDP: https://www.mathworks.com/matlabcentral/fileexchange/29800-scenes-objects-classification-toolbox 

2. Model compression and acceleration. 

As the first author, I proposed Modulated neural networks, a learnable version of Gabor CNNs, to significantly compress deep models. We further developed a series of binary neural networks (BNNs), with more than 20 top tier conference/journal papers published, such as in IJCV/PAMI, CVPR (oral, highlight), and AAAI (oral). We published the first book in the field of BNNs. Our 1-bit object detector achieved lossless mAP performance with more than 10-times speed-up over full-precision counterparts on low-power ARM processors.  We received long-term project support with an outstanding final project evaluation from Huawei. 16 of our BNNs/ low-bit algorithms/models were integrated into Huawei Noah/Bolt and MindSpore. Our lossless low-bit quantization methods were successfully and widely used in industry. Our work was cited by Christoph Meinel, Academician of the German Academy of Engineering (e.g. state-of-the-art and improved training strategy). Our BNN object detectors were embedded into intelligent cameras for Mine site abnormal behavior and building vibration monitoring by Jingying shuzhi Technology Co. Ltd. We are one of the biggest groups on model compression and acceleration in the world, contributing about 20% top tier conference/journal papers in the field of BNNs (recent 3 years).

[1] Zhao Junhe, Gu Jiaxin, Jiang Xiaolong, Zhang Baochang*, Guo Guodong, Liu Jianzhuang. Bayesian optimized 1-bit CNNs[C]//Proceedings of the IEEE/CVF International Conference on Computer Vision. 2019: 4909-4917.

[2] Xu Sheng, Zhao Junhe, Lv Jinhu, Zhang Baochang*, Han Shumin, Doermann David. Layer-wise searching for 1-bit detectors[C]//Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2021: 5682-5691. 

[3] Zhao Junhe, Xu Sheng, Zhang Baochang*, Gu Jiaxin, Doermann David, Guo Guodong. Towards compact 1-bit CNNs via Bayesian learning[J]. International Journal of Computer Vision, 2022: 1-25.

[4] Chen Hanlin, Zhuo Li’an, Zhang Baochang*, Zheng Xiawu, Liu Jianzhuang, Doermann David, Ji Rongrong. Binarized neural architecture search for efficient object recognition[J]. International Journal of Computer Vision, 2021, 129: 501-516.

[5] Lin Mingbao, Ji Rongrong, Sun Xiaoshuai, Zhang Baochang, Huang Feiyue, Tian Yonghong, Tao Dacheng. Fast class-wise updating for online hashing[J]. IEEE Transactions on Pattern Analysis and Machine Intelligence, 2020, 44(5): 2453-2467.

[6] Li Yanjing, Xu Sheng, Cao Xianbin*, Zhuo Li’an, Zhang Baochang*, Wang Tian, Guo Guodong. DCP-NAS: Discrepant Child-Parent Neural Architecture Search for 1-bit CNNs. International Journal of Computer Vision, 2023. 

[7] Liu Chunlei, Ding Wenrui, Hu Yuan, Zhang Baochang*, Liu Jianzhuang, Guo Guodong, Doermann David. Rectified binary convolutional networks with generative adversarial learning[J]. International Journal of Computer Vision, 2021, 129: 998-1012.

[8] Xu Sheng, Yanjing Li, Mingbao Lin, Peng Gao, Guodong Guo, Jinhu Lu, Zhang Baochang*. Q-DETR: An Efficient Low-Bit Quantized Detection Transformer[C]//Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2023

The project related to our work can refer to my student Yanjing Li and Sheng xu github: https://github.com/YanjingLi0202, https://github.com/SteveTsui 

3. Cogradient descent algorithm for decoupled learning.
 
We discovered the independence assumption defect of the classical gradient descent algorithm, and proposed a co-gradient descent algorithm to decouple the deep model parameters and enhance feature representational capabilities. Based on the co-gradient descent algorithm, improved feature enhancement, and detector fusion methods, we won the first place prizes in three international conference competitions (tiny object detection, the COCO object detection, and Pollen recognition challenges), including the prestigious computer vision and pattern recognition conferences ECCV and ICPR. Our algorithm can also be used to build an associative adversarial learning method, which can improve the model's defense ability by 13.9%. Our method was integrated into the Baidu paddlepaddle deep learning platform (one of the largest ones in China) as a basic architecture learning method. We developed the first 2D CAD image parsing method, which was successfully used by China Unicom. The method is considered as “the first work to decouple hidden variables” by Prof. Dacheng Tao, an Australian Academy of Science Fellow. The related works have been published in CVPR (oral 4.59%), ICCV, AAAI and IJCV.


[1] Zhuo Li’an, Zhang Baochang*, Yang Linlin, Chen Hanlin, Ye Qixiang, Doerman David, Ji Rongrong, Guo Guodong. Cogradient descent for bilinear optimization[C]//Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2020: 7959-7967.

[2] Wang Runqi, Liu Zhen, Zhang Baochang*, Guo Guodong, Doermann David. Few-Shot Learning with Complex-Valued Neural Networks and Dependable Learning[J]. International Journal of Computer Vision, 2023, 131(1): 385-404. 

[3] Wang Runqi, Duan Xiaoyue, Kang Guoliang, Liu Jianzhuang, Lin Shaohui, Xu Songcen, Lu Jinhu, Zhang Baochang*. AttriCLIP: A Non-Incremental Learner for Incremental Knowledge Learning[C]//Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2023. 

[4] Zheng Xiawu, Ji Rongrong, Chen Yuhang, Wang Qiang, Zhang Baochang, Chen Jie, Ye Qixiang, Huang Feiyue, Tian Yonghong. Migo-nas: Towards fast and generalizable neural architecture search[J]. IEEE Transactions on Pattern Analysis and Machine Intelligence, 2021, 43(9): 2936-2952.

[5] Wang Runqi, Zheng Hao, Duan Xiaoyue, Liu Jianzhuang, Lu Yuning, Wang Tian, Xu Songcen, Zhang Baochang*. Few-Shot Learning with Visual Distribution Calibration and Cross-Modal Distribution Alignment[C]//Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2023

[6] Mingyuan Mao, Yuxin Tian, Baochang Zhang*, Qixiang Ye, Wanquan Liu, David S. Doermann: iffDetector: Inference-Aware Feature Filtering for Object Detection. IEEE Trans. Neural Networks Learn. Syst. 33(11): 6494-6503 (2022)

[7] Chunlei Liu, Wenrui Ding*, Jinyu Yang, Vittorio Murino, Baochang Zhang*, Jungong Han, Guodong Guo: Aggregation Signature for Small Object Tracking. IEEE Trans. Image Process. 29: 1738-1747 (2020)

[8] Y. Feng, B. Zhang, X. Wang, X. Ying, J. Liu, M. Mao, S. Xu, Baochang Zhang*, Shumin Han*, TOD Challenge on 1st Tiny Person Detection, European Conference on Computer Vision 2020

The project related to our work can refer to my student Sheng xu github: https://github.com/SteveTsui 

4. Summary of my contributions

I have published three books and about 100 papers in top-tier journals and conferences with approximately 13,000 citations on Google Scholar. I have been listed as one of the world's top 1% scholars (recognized by Stanford and Elsevier) in 2023. I received one national teaching award, four first-place prizes from provincial and national associations, and three first-place prizes in international competitions, including ECCV and ICPR. I was supported by the Program for the New Century Excellent Talents from the Ministry of Education of China in 2013, the Shenzhen Overseas High-Level Talent Program in 2017, and the Jiangxi One-Thousand Talent Program in 2023.

