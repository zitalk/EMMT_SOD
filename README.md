# EMMT_SOD
The official repository of "Efficient Multi-Modal Tuning via Visual Prompts for Salient Object Detection."
The code and results can be downloaded from this link: https://pan.baidu.com/s/1K3_XnM8iSrmBGwmyVpokjw?pwd=emmt 
Extraction code: emmt

# Results
## Quantitative results of different RGB SOD methods
The symbols ↑/↓ indicate that a higher/lower score is better, and the best performances are in bold.
| Method | Params ↓ | PASCAL-S Sm ↑ | PASCAL-S Fβω ↑ | PASCAL-S MAE ↓ | PASCAL-S Em ↑ | HKU-IS Sm ↑ | HKU-IS Fβω ↑ | HKU-IS MAE ↓ | HKU-IS Em ↑ | DUTS-TE Sm ↑ | DUTS-TE Fβω ↑ | DUTS-TE MAE ↓ | DUTS-TE Em ↑ | DUT-OMRON Sm ↑ | DUT-OMRON Fβω ↑ | DUT-OMRON MAE ↓ | DUT-OMRON Em ↑ |
|---------|----------|-------------|--------------|--------------|------------|------------|--------------|------------|------------|------------|------------|------------|------------|------------|------------|------------|------------|
| GateNet | 128.6 | 0.854 | 0.804 | 0.071 | 0.900 | 0.915 | 0.880 | 0.033 | 0.955 | 0.885 | 0.809 | 0.040 | 0.928 | 0.838 | 0.729 | 0.055 | 0.876 |
| MINet | 47.6 | 0.854 | 0.818 | 0.066 | 0.901 | 0.919 | 0.897 | 0.029 | 0.960 | 0.884 | 0.825 | 0.037 | 0.927 | 0.833 | 0.738 | 0.056 | 0.869 |
| VST | 44.1 | 0.871 | 0.827 | 0.062 | 0.918 | 0.928 | 0.897 | 0.029 | 0.968 | 0.896 | 0.828 | 0.037 | 0.939 | 0.850 | 0.755 | 0.058 | 0.888 |
| SGL-KRN | 72.4 | 0.854 | 0.823 | 0.070 | 0.900 | 0.921 | 0.904 | 0.028 | 0.961 | 0.893 | 0.847 | 0.034 | 0.939 | 0.846 | 0.765 | 0.049 | 0.885 |
| ZoomNet | 32.4 | 0.869 | 0.844 | 0.057 | 0.917 | **0.931** | 0.918 | **0.023** | 0.967 | 0.900 | 0.854 | 0.033 | 0.936 | 0.841 | 0.755 | 0.053 | 0.872 |
| MENet | -- | 0.872 | **0.847** | **0.053** | 0.910 | 0.927 | 0.917 | **0.023** | 0.960 | 0.905 | 0.870 | 0.028 | 0.938 | 0.859 | 0.785 | **0.046** | 0.888 |
| BSNet | 53.0 | 0.842 | 0.800 | 0.066 | 0.897 | 0.906 | 0.891 | 0.031 | 0.954 | 0.856 | 0.797 | 0.043 | 0.915 | 0.815 | 0.724 | 0.058 | 0.863 |
| **Ours** | **4.4** | **0.881** | **0.847** | **0.053** | **0.920** | **0.931** | **0.921** | 0.024 | **0.962** | **0.915** | **0.881** | **0.027** | **0.949** | **0.862** | **0.790** | **0.046** | **0.893** |

## Quantitative results of different Light Field SOD methods
The symbols ↑/↓ indicate that a higher/lower score is better, and the best performances are in bold.
| Method | Params ↓ | DUTLF-V2 Sm ↑ | DUTLF-V2 Fβω ↑ | DUTLF-V2 MAE ↓ | DUTLF-V2 Em ↑ |
|--------|---------|--------------|--------------|--------------|--------------|
| SA-Net | 66.9  | 0.857 | 0.792 | 0.046 | 0.906 |
| PANet | 15.1  | 0.863 | 0.785 | 0.048 | 0.897 |
| LFBCNet | 11.6  | 0.885 | 0.821 | 0.042 | 0.919 |
| ESCNet | 32.8  | 0.881 | 0.817 | 0.042 | 0.909 |
| CDINet | -     | 0.905 | 0.861 | 0.033 | 0.933 |
| **Ours** | **4.4**  | **0.919** | **0.884** | **0.027** | **0.951** |

## Quantitative results of different RGB-D SOD methods
The symbols ↑/↓ indicate that a higher/lower score is better, and the best performances are in bold.
| Method | Params ↓ | SIP Sm ↑ | SIP Fβ ↑ | SIP MAE ↓ | SIP Em ↑ | STERE Sm ↑ | STERE Fβ ↑ | STERE MAE ↓ | STERE Em ↑ | NJU2K Sm ↑ | NJU2K Fβ ↑ | NJU2K MAE ↓ | NJU2K Em ↑ |
|--------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|
| CMINet | 196.2  | 0.899  | 0.872  | 0.040  | **0.937**  | 0.918  | 0.886  | 0.032  | 0.948  | 0.929  | 0.910  | 0.029  | **0.953**  |
| UCNet-CVAE | 31.3  | 0.882  | 0.850  | 0.045  | 0.927  | 0.906  | 0.878  | 0.036  | 0.945  | 0.904  | 0.886  | 0.038  | 0.943  |
| DCF | 12.0  | 0.876  | 0.838  | 0.052  | 0.915  | 0.902  | 0.867  | 0.039  | 0.902  | 0.912  | 0.886  | 0.036  | 0.944  |
| SSLSOD | 74.2  | 0.868  | 0.830  | 0.058  | 0.903  | 0.885  | 0.845  | 0.047  | 0.885  | 0.901  | 0.872  | 0.042  | 0.932  |
| CCFENet | 28.7  | 0.882  | 0.857  | 0.047  | 0.920  | 0.906  | 0.881  | 0.035  | 0.906  | 0.917  | 0.897  | 0.032  | 0.949  |
| DIGR-Net | 166.7  | 0.885  | 0.841  | 0.052  | 0.913  | 0.916  | 0.870  | 0.037  | 0.916  | **0.933**  | 0.904  | **0.028**  | **0.953**  |
| CAVER | 55.8  | 0.893  | 0.864  | 0.042  | 0.933  | 0.913  | 0.882  | 0.033  | 0.949  | 0.921  | 0.901  | 0.031  | **0.953**  |
| LSNet | 4.6  | 0.886  | 0.847  | 0.050  | 0.920  | 0.871  | 0.816  | 0.055  | 0.908  | 0.911  | 0.878  | 0.039  | 0.939  |
| **Ours** | **4.4**  | **0.908**  | **0.884**  | **0.036**  | 0.908  | **0.924**  | **0.894**  | **0.030**  | **0.951**  | 0.929  | **0.907**  | 0.029  | **0.953**  |

## Quantitative results of different RGB-T SOD methods
The symbols ↑/↓ indicate that a higher/lower score is better, and the best performances are in bold.
| Method  | Params ↓ | VT821 Sm ↑ | VT821 Fβω ↑ | VT821 MAE ↓ | VT821 Em ↑ | VT1000 Sm ↑ | VT1000 Fβω ↑ | VT1000 MAE ↓ | VT1000 Em ↑ | VT5000 Sm ↑ | VT5000 Fβω ↑ | VT5000 MAE ↓ | VT5000 Em ↑ |
|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|
| ECFFNet | -     | 0.877  | 0.799  | 0.035  | 0.907  | 0.924  | 0.883  | 0.022  | 0.910  | 0.875  | 0.800  | 0.038  | 0.910  |
| CGFNet  | 69.9  | 0.880  | 0.829  | 0.038  | 0.918  | 0.923  | 0.900  | 0.023  | 0.955  | 0.883  | 0.831  | 0.035  | 0.924  |
| APNet   | 30.4  | 0.868  | 0.791  | 0.034  | 0.898  | 0.922  | 0.882  | 0.022  | 0.949  | 0.876  | 0.805  | 0.035  | 0.913  |
| CCFENet | 28.7  | **0.900**  | **0.852**  | **0.027**  | **0.932**  | 0.934  | 0.910  | 0.018  | 0.964  | 0.896  | 0.849  | 0.030  | 0.935  |
| TNet    | 87.0  | 0.899  | 0.841  | 0.030  | 0.928  | 0.929  | 0.895  | 0.021  | 0.957  | 0.895  | 0.840  | 0.033  | 0.931  |
| LSNet   | 4.6   | 0.879  | 0.808  | 0.033  | 0.911  | 0.926  | 0.886  | 0.023  | 0.954  | 0.877  | 0.804  | 0.037  | 0.916  |
| CAVER   | 55.8  | 0.891  | 0.835  | 0.033  | 0.926  | 0.936  | 0.909  | **0.017**  | 0.965  | 0.892  | 0.835  | 0.032  | 0.930  |
| TMMANet | 141   | 0.880  | 0.804  | 0.032  | 0.908  | 0.939  | 0.908  | 0.018  | 0.946  | 0.898  | 0.836  | 0.030  | 0.929  |
| **Ours** | **4.4**  | **0.901**  | 0.843  | 0.034  | 0.925  | **0.941**  | **0.916**  | **0.017**  | **0.967**  | **0.901**  | **0.853**  | **0.028**  | **0.936**  |

# BibTeX
```
@article{zhang2025parameter,
  title={Efficient Multi-Modal Tuning via Visual Prompts for Salient Object Detection},
  author={Zhang, Zixuan and Shi, Fan and Jia, Chen and Wang, Mianzhao and Louis, Assale Adje and Cheng, Xu},
  journal={ACM Transactions on Multimedia Computing, Communications, and Applications},
  year={2025},
}
```
