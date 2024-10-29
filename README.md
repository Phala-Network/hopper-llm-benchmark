# Confidential Computing on nVIDIA Hopper GPUs: A Performance Benchmark Study

This report evaluates the performance impact of enabling Trusted Execution Environments (TEE) on nVIDIA Hopper GPUs for large language model (LLM) inference tasks. We benchmark the overhead introduced by TEE mode across various LLMs and token lengths, with a particular focus on the bottleneck caused by CPU-GPU data transfers via PCIe. Our results indicate that while there is minimal computational overhead within the GPU, the overall performance penalty is primarily attributable to data transfer. For the majority of typical LLM queries, the overhead remains below 7%, with larger models and longer sequences experiencing nearly zero overhead.

If you use this benchmark in your research, we would appreciate it if you would cite us:

```
@misc{zhu2024confidentialcomputingnvidiahopper,
      title={Confidential Computing on nVIDIA Hopper GPUs: A Performance Benchmark Study},
      author={Jianwei Zhu and Hang Yin and Peng Deng and Aline Almeida and Shunfan Zhou},
      year={2024},
      eprint={2409.03992},
      archivePrefix={arXiv},
      primaryClass={cs.DC},
      url={https://arxiv.org/abs/2409.03992},
}
```

## Directory Structure

- The latest version of paper is available both in [this repo](./pdf/main.pdf) and on [Arxiv](https://arxiv.org/abs/2409.03992).
- Raw result data can be found under the [results](./results/) repository.
- Data analysis scripts and the analyzed statistical results are located in the [src](./src/) and [outputs](./outputs/) directories, respectively.
