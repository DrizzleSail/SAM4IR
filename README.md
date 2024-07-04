# Distilling Semantic Priors from SAM to Efficient Image Restoration Models.
The pytorch implementation of the paper **[Distilling Semantic Priors from SAM to Efficient Image Restoration Models](https://arxiv.org/pdf/2403.16368)**

In image restoration (IR), leveraging semantic priors from segmentation models has been a common approach to improve performance.  The recent segment anything model (SAM) has emerged as a powerful tool for extracting advanced semantic priors to enhance IR tasks.  However, the computational cost of SAM is prohibitive for IR, compared to existing smaller IR models. The incorporation of SAM for extracting semantic priors considerably hampers the model inference efficiency. To address this issue, we propose a general framework to distill SAM's semantic knowledge to boost exiting IR models without interfering with their inference process. Specifically, our proposed framework consists of the semantic priors fusion (SPF) scheme and the semantic priors distillation (SPD) scheme. SPF fuses two kinds of information between the restored image predicted by the original IR model and the semantic mask predicted by SAM for the refined restored image. SPD leverages a self-distillation manner to distill the fused semantic priors to boost the performance of original IR models. Additionally, we design a semantic-guided relation (SGR) module for SPD, which ensures semantic feature representation space consistency to fully distill the priors. We demonstrate the effectiveness of our framework across multiple IR models and tasks, including deraining, deblurring, and denoising.

- The code will be released soon.

### Installation
This implementation based on [BasicSR](https://github.com/xinntao/BasicSR) which is a open source toolbox for image/video restoration tasks and [HINet](https://github.com/megvii-model/HINet) 

```python
python 3.9.5
pytorch 1.11.0
cuda 11.3
```

### Citations
If SAM4IR helps your research or work, please consider citing NAFNet.

```
@inproceedings{zhang2024distilling,
  title={Distilling Semantic Priors from SAM to Efficient Image Restoration Models},
  author={Zhang, Quan and Liu, Xiaoyu and Li, Wei and Chen, Hanting and Liu, Junchao and Hu, Jie and Xiong, Zhiwei and Yuan, Chun and Wang, Yunhe},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={25409--25419},
  year={2024}
}
```

### Contact

If you have any questions, please contact quanz7165@gmail.com


