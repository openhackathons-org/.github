[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) 


#  Open Hackathons Official Training Materials

The Open Hackathons program presents a unique opportunity for scientists, researchers, and developers to build collaborations and learn the hands-on skills needed to accelerate and optimize their applications using a variety of programming models, libraries, and tools. Currently, we offer two types of events: Hackathons and Bootcamps.

Bootcamps are designed to help build confidence and eventually prepare developers to participate in [Hackathons](http://openhackathons.org/)
This repository contains bootcamp material for high performance computing (HPC), Artificial Intelligence (AI), and the convergence of both.

- __HPC__ :: 
This bootcamp content focuses on how to follow the “Analyze, Parallelize, and Optimize” cycle to write parallel code using different parallel programming models for accelerating HPC simulations.

| Lab      | Description |
| ----------- | ----------- |
| [N-Ways](https://github.com/openhackathons-org/nways_accelerated_programming)      | This Bootcamp will cover multiple GPU programming models and choose the one that best fits your needs. The material supports different programming ,languages including C ( CUDA C, OpenACC C, OpenMP C, C++ stdpar ),  Fortran ( CUDA Fortran, OpenACC Fortran, OpenMP Fortran, ISO DO CONCURRENT ) Python ( Numba, CuPy )       |
| [HPC Profiler](https://github.com/openhackathons-org/HPC_Profiler)  | This repository contains learning materials and exercises for NVIDIA Nsight Tools. Goal is to learn how to profile your application with NVIDIA Nsight Systems, Comput,e and NVTX API calls to find performance limiters and bottlenecks and apply incremental parallelization strategies |
| [C++ Standard Parallelism](https://github.com/openhackathons-org/cpp_hpc_tutorial)  | This repository contains learning materials and exercises for C++ Standard Parallelism. The content covers the step-by-step process of accelerating a portable HPC application with CPUs and GPUs using the parallelism and concurrency features of the C++17 and C++20 standards. The goal is to learn about C++ concurrency features like threads, atomics, barriers, and parallel algorithms. This forked content has been tested. The owners of the material are Gonzalo Brito and Jonas Latt|


- __Convergence of HPC and AI__ :: 
The bootcamp content focuses on how AI can accelerate HPC simulations by introducing concepts of Deep Neural Networks, including Physics Informed Neural Networks, neural operators and techniques to visualise physically accurate outputs from the trained models. 

| Lab      | Description |
| ----------- | ----------- |
| [End to End AI for Science](https://github.com/openhackathons-org/End-to-End-AI-for-Science)      | This bootcamp provides a step-by-step overview of the fundamentals of deep neural networks, walks attendees through the hands-on experience of building and improving deep learning models using a framework that uses the fundamental laws of physics to model the behavior of complex systems, and enables attendees to visualize the physically accurate outputs of the trained model in near real-time. |


- __AI__ ::
The bootcamp content focuses on using popular accelerated AI frameworks and using optimization techniques to get maximum performance from accelerators like GPUs.


| Lab      | Description |
| ----------- | ----------- |
| [AI Profiler](https://github.com/openhackathons-org/AI-Profiler)   | Learn how to optimize a Deep Neural Network (DNN) training  using profiling tools   |
| [NVIDIA NIM Bootcamp](https://github.com/openhackathons-org/NIM-Bootcamp) | The NVIDIA NIM bootcamp is designed to help developers get started with NVIDIA® NIM™ microservices by building real-world GenAI applications. The labs guide participants through setting up NIM Docker containers and utilizing REST API endpoints for serving inference requests. Additionally, attendees will explore fine-tuning models using Parameter Efficient Fine-Tuning (PEFT) techniques such as LoRA, with hands-on experience in fine-tuning adapters for the LLaMA-3 8B model. Participants will also utilise multimodal NIM and put multiple NIM in agentic workflows using LangGraph. The bootcamp gives a hands-on overview of deploying NIM Blueprints. |
| [Agentic AI Bootcamp](https://github.com/openhackathons-org/bootcamp-challenge-public-nim) | Agentic AI employs sophisticated reasoning to solve complex problems, utilizing data from multiple sources to analyze, strategize, and complete tasks independently. There are many powerful building blocks that developers and researchers can use to enable and accelerate the development and deployment of their agentic AI workflows. The Agentic AI Bootcamp covers some of these powerful tools, including Model Context Protocol (MCP), an open protocol providing a standardized method for connecting AI models to various data sources and tools; NVIDIA® NIM™, a set of easy-to-use microservices that provides pre-optimized models and industry-standard APIs for building powerful AI agents, co-pilots, chatbots, and assistants; and LangGraph, an open-source library for complex, stateful, and cyclic workflows for AI agents. Attendees are guided through the creation of MCP servers based on Stdio/HTTP using the high/low level MCP SDKs, building MCP clients to interact with MCP Servers, and using MCP Clients/Servers with NVIDIA NIM in LLM/Agentic workflows. Attendees will then apply these learned skills in a hands-on challenge to replace parts of an existing workflow with MCP.

# System Requirements
Each repository contains docker/singularity/conda definition files. Follow the README files inside each on how to build the container and run the labs inside it.

# Contribution
- The repository uses the Apache 2.0 license. For more details on folder structure, developers may refer to the CONTRIBUTING.md file.

# Feature Request or filing issues
- Bootcamp users may request newer training material or file a bug by filing a GitHub issue
- Please do go through the existing list of issues to get more details of upcoming features and bugs currently being fixed.

## General Troubleshooting

- All materials developed are tested with the latest GPU Architectures (V100, A100). Most labs, unless specified explicitly, are expected to work even on older GPU architectures and with lesser compute and memory capacity, like the one present even in laptops. There will be a change in performance results observed based on the GPU used. In case you see any issue using the material on another GPU, please file an issue in GitHub mentioning the details of the GPU and the CUDA Driver version installed.
- The material developed is tested inside a container environment, like Docker and Apptainer. In case the users don't have a container environment in the cluster, they can explicitly look at the steps mentioned in the Dockerfile and Singularity scripts and install the dependencies manually.
- Most bootcamps are jupyter based and by default, the Dockerfile and Singularity script run the Jupyter notebook at port 8888. In a multi-tenancy environment, the admins are requested to explicitly map the ports to individual users; else will result in port conflict issues. We recommend having installations of interactive interfaces to remote computing resources like [Open OnDemand](https://openondemand.org/) or [JupyterHub](https://jupyter.org/hub) coupled with a scheduler (SLURM, Kubernetes, etc ) to automatically map these resources. 

## Join OpenACC Community
Please join [OpenACC Slack Channel](https://openacclang.slack.com/messages/openaccusergroup).
