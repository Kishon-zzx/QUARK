# [ICCAD'25] QUARK: Quantization-Enabled Circuit Sharing for Transformer Acceleration by Exploiting Common Patterns in Nonlinear Operations

[Zhixiong Zhao](https://kishon-zzx.github.io/)*, Haomin Li*, Fangxin Liu, Yuncheng Lu, Zongwu Wang, Tao Yang, Li Jiang, and Haibing Guan

---

> **Abstract:** Transformer-based models have revolutionized computer vision (CV) and natural language processing (NLP) by achieving state-of-the-art performance across a range of benchmarks. However, nonlinear operations in models significantly contribute to inference latency, presenting unique challenges for efficient hardware acceleration. To this end, we propose QUARK, a quantization-enabled FPGA acceleration framework that leverages common patterns in nonlinear operations to enable efficient circuit sharing, thereby reducing hardware resource requirements. QUARK targets all nonlinear operations within Transformer-based models, achieving high-performance approximation through a novel circuit-sharing design tailored to accelerate these operations. Our evaluation demonstrates that QUARK significantly reduces the computational overhead of nonlinear operators in mainstream Transformer architectures, achieving up to a 1.96× end-to-end speedup over GPU implementations. Moreover, QUARK lowers the hardware overhead of nonlinear modules by more than 50% compared to prior approaches, all while maintaining high model accuracy---and even substantially boosting accuracy under ultra-low-bit quantization.

![](figs/overview.png)

![](figs/hardware.png)

# <a name="results"></a>🔎 Results

<details>
<summary>Algorithm Accuracy Results (click to expand) </summary>
<li> Performance comparison of various methods on ImageNet (Table 1 from the main paper). 
 
<p align="center">
    <img src="figs/results_alg.png" >
</p>

</details>

<details>
<summary>Hardware Evaluation (click to expand) </summary>
<li> Comparison of hardware overhead with SOTA FPGA implementations. \textbf{*} indicates the resource consumption of non-shared components, excluding shared resources in nonlinear operators. (Table 4 from the main paper). 
 
<p align="center">
    <img src="figs/results_fpga.png" >
</p>

</details>

## Citation

If you find the code helpful in your research or work, please cite the following paper.

```
@inproceedings{zhao2025quark,
    title={QUARK: Quantization-Enabled Circuit Sharing for Transformer Acceleration by Exploiting Common Patterns in Nonlinear Operations},
    author={Zhao, Zhixiong and Li, Haomin and Liu, Fangxin and Lu, Yuncheng and Wang, Zongwu and Yang, Tao and Jiang, Li and Guan, Haibing},
    booktitle={2025 IEEE/ACM International Conference On Computer Aided Design (ICCAD)},
    pages={1--9},
    year={2025},
    organization={IEEE}
  }
```