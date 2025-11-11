---
layout: post
title: "Hello World - Starting My CUDA Journey"
date: 2025-11-11
categories: cuda intro
---
#### TL;DR:

This blog details my plan to go from zero CUDA knowledge to advanced GPU programming for deep learning. 

## Intro

This is the first posting of hopefully a long-running series documenting my journey in learning CUDA, parallel programming and a deep knowledge in DL. I am a junior machine learning engineer, I have studied computer science and currently doing a Master's, and I have never been exposed to GPU programming or C++ in my studies or work life. 

I avoided C++ because it looked horrible in one of my modules and stuck to Python because it is simple and easy. However, I have read and heard how challenging C++ is and GPU programming so I want to commit to learning and hopefully teach others along the way.


## Why CUDA 

I enjoy working on machine learning algorithms and currently exploring deep learning for some work projects. But I have no understanding on what happens on the backend, how GPUs help make training large models possible. 

I have watched videos and read blog posts and it's amazing how there is a completely undiscovered world (to me) about how the CUDA kernels can influence models in many ways.

This is what sparked my interest in learning CUDA and C++ (also learning something not many people know!).

## What I Aim To Cover 

*This is heavily influenced by X user @sadernoheart & Claude is used for the list*

So, now what I want to tell you what I will cover during the however many months/years I am doing this for. Each segment will contain a topic, what I am covering and a final assignment to show I understand it: 

- C++ foundations
    - Content: Pointers, Memory Management, Structs, Functions, Basic Syntax, Control Flow, RAII, Smart Pointers, STL
    - Assignment: Implementing a basic NN library in C++ (backprop, SGD and basic layers)
- Linear Algebra
    - Content: Matrix multiplication, SVD, Floating-Point Arithmetic, Vectorisation
    - Assignment: Implementing matrix multiplication (GEMM) from scratch
- CUDA Fundamentals
    - Books to read:  PMPP Book, Professional CUDA C programming 
    - Courses: Elliot Arledge's CUDA course, Official NVIDIA Training
    - Content: Thread Hierarchy, Memory Hierarchy, Warp Execution , Divergence, Occupancy , Coalesced Access, Bank Conflicts, Streams, Async Operations
    - Assignment 1: Implement 2D convolution with progressive optimisation (Naive global memory, shared memory tiling, constant memory for filters, register blocking and compare against cuDNN)
    - Assignment 2: Implement basic kernels: reduction, scan, histogram
    - Assignment 3: Implement softmax and cross-entropy kernels
- GPU Architecture Dive 
    - Resources: NVIDIA Architecture Whitepapers, CUDA C++ Best Practices Guide
    - Content: Tensor Cores (WMMA, MMA), SM Architecture, HBM Bandwidth, L2 Cache, Compute vs Memory Bound, Roofline Model
    - Assignment: Profile my convolutional kernel using Nsight compute, create roofline analysis
- PyTorch + CUDA Integration
    - Content: Autograd mechanics, custom autograd functions, torch.nn internals, CUDA kernel integration
    - Assignment: Implement custom attention layer with CUDA kernels in PyTorch
- Implementing Deep Learning in CUDA
    - Content: Attention mechanisms, LayerNorm, Activation functions, loss functions
    - Assignment 1: Implement standard attention in CUDA
    - Assignment 2: Implement fused kernels (LayerNorm+Dropout, GELU)
    - Assignment 3: Implement one SOTA model (transformer) with custom CUDA kernels
- Profiling & optimisation 
    - Content: Nsight Systems, Nsight Compute, Memory throughput analysis, Occupancy tuning 
    - Assignment: Profile end-to-end training, identify and fix bottlenecks.
- Triton Programming
    - Content: Triton Fundamentals, Block-level programming, Auto tuning
    - Assignment 1: Implement Flash Attention in Triton
    - Assignment 2: Compare Triton vs CUDA vs PyTorch
- Quantisation in CUDA
    - Content: INT8, FP16, BF16 kernels, PTQ, QAT, symmetric vs asymmetric, per-tensor vs per-channel, GPTQ, mixed precision training
    - Assignment: Implement quantized convolution and GEMM kernels
- Multi-GPU CUDA
    - Content: NCLL, Multi-GPU patterns, Communication-computation overlap
    - Assignment: Implement data parallelism with NCLL primitives
- Distributed Deep Learning
    - Content: Tensor Parallelism, Pipeline parallelism, 3D parallelism
    - Assignment: Implement tensor parallelism for transformer with CUDA + NCLL
- Inference Optimisation
    - Content: TensorRT, Kernel fusion, Batch processing
    - Assignment: Convert PyTorch model to TensorRT with custom plugins
- Advanced Attention
    - Content: Flash Attention, MQA/GQA, Paged Attention
    - Assignment: Implement Flash Attention in CUDA from scratch
- Mixture of Experts (MoE)
    - Content: Dynamic routing, Load balancing
    - Assignment: Implement MoE layer with efficient CUDA kernels

## My End Goal

That is a lot of things to learn and go through, the chances are I won't go through it all or skip through some but my goal is to go through them all and make some tutorials so other people can learn and follow along.

I want to become an expert in CUDA and GPU programming for deep learning and hopefully this learning path will take me there. 

I started this blog to document my learning journey from zero CUDA knowledge and create a resource for others wanting to learn GPU programming. More importantly to force myself to truly understand by teaching others. 
## Next post 

The next course will be about C++ Foundations, the resources I am using to learn and me teaching them to you! 
