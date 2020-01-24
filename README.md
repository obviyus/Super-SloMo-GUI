# Super-SloMo-GUI
Super-SloMo-GUI is a fork of [avinashpaliwal/Super-SloMo](https://github.com/ avinashpaliwal/Super-SloMo) with [Gooey](https://github.com/chriskiehl/Gooey) thrown on it. The goal is to make it as easy as possible for a layman to use the video-coverter script.

# Super-SloMo [![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://opensource.org/licenses/mit-license.php)
PyTorch implementation of "Super SloMo: High Quality Estimation of Multiple Intermediate Frames for Video Interpolation" by Jiang H., Sun D., Jampani V., Yang M., Learned-Miller E. and Kautz J. [[Project]](https://people.cs.umass.edu/~hzjiang/projects/superslomo/) [[Paper]](https://arxiv.org/abs/1712.00080)

## Results
Results on UCF101 dataset using the [evaluation script](https://people.cs.umass.edu/~hzjiang/projects/superslomo/UCF101_results.zip) provided by paper's author. The `get_results_bug_fixed.sh` script was used. It uses motions masks when calculating PSNR, SSIM and IE.

| Method | PSNR | SSIM | IE |
|------|:-----:|:-----:|:-----:|
| DVF | 29.37 | 0.861 | 16.37 |
| [SepConv](https://github.com/sniklaus/pytorch-sepconv) - L_1 | 30.18 | 0.875 | 15.54 |
| [SepConv](https://github.com/sniklaus/pytorch-sepconv) - L_F | 30.03 | 0.869 | 15.78 |
| SuperSloMo_Adobe240fps | 29.80 | 0.870 | 15.68 |
| **pretrained mine** | **29.77** | **0.874** | **15.58** |
| SuperSloMo | 30.22 | 0.880 | 15.18 |


<img src='./misc/original.gif'>
<img src='./misc/slomo.gif'>

## References:
The original code is forked from [avinashpaliwal/Super-SloMo](https://github.com/ avinashpaliwal/Super-SloMo)

