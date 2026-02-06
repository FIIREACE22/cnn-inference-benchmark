# Benchmark Results Summary

## Experimental Setup

- Model: ResNet18 (pretrained on ImageNet)
- Framework: PyTorch
- Input Size: 224 × 224 RGB images
- Batch Sizes: 1, 8, 16, 32
- Inference Mode: Evaluation (no gradients)

## Hardware

- CPU: Standard x86 CPU
- GPU: CUDA-enabled GPU (if available)

## Key Observations

- GPU inference latency decreases significantly with larger batch sizes due to parallelism.
- CPU latency increases almost linearly with batch size.
- Throughput improves substantially on GPU compared to CPU.
- Warm-up runs are essential for stable GPU measurements.

## Status

Ongoing – additional benchmarking and optimization in progress.
