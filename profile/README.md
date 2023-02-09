[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) 


#  Open Hackathons Official Training Materials

The Open Hackathons program presents a unique opportunity for scientists, researchers, and developers to build collaborations and learn the hands-on skills needed to accelerate and optimize their applications using a variety of programming models, libraries and tools. Currently, we offer two types of events: Hackathons and Bootcamps.

Bootcamps are designed to help build confidence and eventually prepare developers to participate in Hackathons
This repository contains bootcamp material for high performance computing (HPC), artificial intelligence (AI), and convergence of both

GPU Bootcamps are designed to help build confidence in Accelerated Computing and eventually prepare developers to enroll for [Hackathons](http://openhackathons.org/)

This repository consists of GPU bootcamp material for HPC, AI and convergence of both:

- __HPC__ :: 
This bootcamp content focuses on how to follow the “Analyze, Parallelize, and Optimize” cycle to write parallel codes using different parallel programming models for accelerating HPC simulations.

| Lab      | Description |
| ----------- | ----------- |
| [N-Ways](https://github.com/gpuhackathons-org/openbootcamp/tree/master/hpc/nways)      | This Bootcamp will cover multiple GPU programming models and choose the one that best fits your needs. The material supports different programming langauges including C ( CUDA C, OpenACC C, OpenMP C, C++ stdpar ),  Fortran ( CUDA Fortran, OpenACC Fortran, OpenMP Fortran, ISO DO CONCURRENT ) Python ( Numba, CuPy )       |
| [OpenACC](https://github.com/gpuhackathons-org/openbootcamp/tree/master/hpc/openacc)   | The Bootcamp will cover how to write portable parallel program that can run on multicore CPUs and accelerators like GPUs and how to apply incremental parallelization strategies using OpenACC       |
| [Multi GPU Programming Model](https://github.com/openhackathons-org/gpubootcamp/tree/master/hpc/multi_gpu_nways)   | This bootcamp will cover scaling applications to multiple GPUs across multiple nodes. Moreover, understanding of the underlying technologies and communication topology will help us utilize high-performance NVIDIA libraries to extract more performance out of the system     |
| [HPC Profiler](https://github.com/openhackathons-org/HPC_Profiler)  | his repository contains learning materials and exercises for NVIDIA Nsight Tools. Gola is to learn how to profile your application with NVIDIA Nsight Systems,Compute and NVTX API calls to find performance limiters and bottlenecks and apply incremental parallelization strategies |


- __Convergence of HPC and AI__ :: 
The bootcamp content focuses on how AI can accelerate HPC simulations by introducing concepts of Deep Neural Networks, including data pre-processing, techniques on how to build, compare and improve accuracy of deep learning models. 

| Lab      | Description |
| ----------- | ----------- |
| [Weather Pattern Recognition](https://github.com/openhackathons-org/gpubootcamp/tree/master/hpc_ai/ai_science_climate)      | This Bootcamp will introduce developers to fundamentals of AI and how data driven approach can be applied to Climate/Weather domain |
| [CFD Flow Prediction](https://github.com/openhackathons-org/gpubootcamp/tree/master/hpc_ai/ai_science_cfd)      | This Bootcamp will introduce developers to fundamentals of AI and how they can be applied to CFD (Computational Fluid Dynamics) |
| [PINN](https://github.com/openhackathons-org/gpubootcamp/tree/master/hpc_ai/PINN)      | This Bootcamp will introduce developers to fundamentals of using Physics Informed Neural Network and how they can be applied to different scientific domains using Nvidia Modulus |

- __AI__ ::
The bootcamp content focuses on using popular accelerated AI frameworks and using optimization techniques to get max performance from accelerators like GPU.


| Lab      | Description |
| ----------- | ----------- |
| [End to End Computer Vision](https://github.com/openhackathons-org/End-to-End-Computer-Vision) | This repository contains the material for the end-to-end computer vision bootcamp, the goal of which is to build a complete end-to-end computer vision pipeline for an object detection application. This bootcamp will introduce participants to multiple NVIDIA® SDKs, most notably NVIDIA TAO Toolkit, NVIDIA TensorRT™, NVIDIA Triton™ Inference Server, and NVIDIA DeepStream SDK. Participants will also have hands-on experience in data preprocessing, model training, optimization, and deployment at scale       |
| [AI Profiler](https://github.com/openhackathons-org/AI-Profiler)   | Learn how optimizing a Deep Neural Network (DNN) training  using profiling tools   |

# System Requirements
Each lab contains docker and singularity definition files. Follow the readme files inside each on how to build the container and run the labs inside it.

# Contribution
- The repository uses Apache 2.0 license. For more details on folder structure developers may refer to CONTRIBUTING.md file.

## Authors and Acknowledgment

See [Contributors](https://github.com/gpuhackathons-org/contributors) for a list of contributors towards this repositories.


# Feature Request or filing issues
- Bootcamp users may request for newer training material or file a bug by filing a github issues
- Please do go through the existing list of issues to get more details of upcoming features and bugs currently being fixed)

## General Troubleshooting

- All materials developed are tested with latest GPU Architectures (V100, A100). Most labs unless specified explicitly are expected to work even on older GPU architectures and with lesser compute and memory capacity like the one present even in laptops. There will be change in performance results observed based on GPU used. In case you see any issue using the material on other GPU please file an issue in Github mentioning the details of GPU and CUDA Driver version installed.
- The material developed are tested inside container environment like Docker and Singularity. In case the users don't have container environment in the cluster, they can explicitly look at the steps mentioned in the Dockerfile and Singularity scripts and install the dependenciesmanually.
- Most bootcamps are jupyter based and by default the Dockerfile and Singularity script runs the jupyter notebook at port 8888. In a munti-tenancy environment the admins are requested to explicitly map the ports to individual users else will result into port conflict issues. We recommend having installations of interactive interface to remote computing resources like [Open OnDemand](https://openondemand.org/) or [JupyterHub](https://jupyter.org/hub) coupled with scheduler (SLURM, Kubernetes etc ) to do these resources mapping automatically. 

## Join OpenACC Community
Please join [OpenACC Slack Channel](https://openacclang.slack.com/messages/openaccusergroup).
