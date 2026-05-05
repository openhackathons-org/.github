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


- __AI for science__ :: 
The bootcamp content applies AI to scientific research and engineering across domains that span digital biology, molecular design, and materials science—including structure–property relationships, discovery workflows, and simulation at multiple scales. The material also emphasizes physics-informed modeling and large-scale scientific computing to connect mechanistic insight with data-driven methods, helping participants build models that are faithful to the science question and practical to run on modern GPU infrastructure.

| Lab      | Description |
| ----------- | ----------- |
| [AI-Powered Drug Discovery Bootcamp](https://github.com/openhackathons-org/AI-Powered-Drug-Discovery-Bootcamp) | The AI-Powered Drug Discovery Bootcamp provides attendees with an overview of the NVIDIA® BioNeMo™ platform for digital biology, explores MolMIM (Molecular Masked Image Modeling), an AI model for small molecule drug discovery that can generate novel, valid molecules with specific properties, and highlights DiffDock, an AI model that predicts the three-dimensional structure of a protein-ligand complex, a crucial step in the drug discovery process.<br><br>Attendees are guided through comprehensive tutorials and participate in an exciting hands-on challenge, generating and optimizing novel molecular structures with a focus on their potential as therapeutic agents, to gain valuable practical experience. |
| [AI-Powered Physics Bootcamp](https://github.com/openhackathons-org/AI-Powered-Physics-Bootcamp) | The AI-Powered Physics Bootcamp helps participants revolutionize their approach to computational physics problems by combining traditional physics-based modeling with modern artificial intelligence (AI) to tackle real-world scientific computing challenges orders of magnitude faster than traditional simulation methods.<br><br>Attendees are introduced to NVIDIA® PhysicsNeMo, an open-source Python framework for building, training, and fine-tuning physics AI models, and guided through progressive challenges to solve complex scientific problems by combining physics-based partial differential equations (PDEs) with AI.<br><br>Participants gain hands-on practical skills to accelerate their own research and engineering workflows, whether they are optimizing designs, forecasting complex phenomena, or solving multi-physics problems. Afterwards, attendees can confidently apply physics-informed AI to their domain, understand when to leverage physics constraints versus data-driven approaches, and how to visualize and validate their results. |
| AI-Powered Atomistic Simulation for Chemistry And Materials Science Innovation | *Coming soon* |


- __AI__ ::
The bootcamp content focuses on using popular accelerated AI frameworks and using optimization techniques to get maximum performance from accelerators like GPUs.


| Lab      | Description |
| ----------- | ----------- |
| [Profiling AI Software Bootcamp](https://github.com/openhackathons-org/Profiling-AI-Software-Bootcamp)   | The Profiling AI Software Bootcamp covers the process and tools for profiling AI and machine learning applications to fully utilize high-performance systems. Attendees will learn to profile applications using NVIDIA Nsight™ Systems, a system-wide performance analysis tool; analyze and identify optimization opportunities; and improve application performance to scale efficiently across systems of any size and number of CPUs and GPUs. Additionally, this bootcamp will walk through the system topology to learn the dynamics of FP8 precision, multi-GPU, and multi-node connections and architecture.   |
| [Agentic AI Bootcamp](https://github.com/openhackathons-org/agentic-ai-bootcamp) | Agentic AI uses advanced reasoning and data from multiple sources to analyze, plan, and complete tasks independently. Developers can leverage key building blocks to accelerate these workflows. The Agentic AI Bootcamp introduces tools such as Agent Skills (modular resources that add capabilities), Model Context Protocol (MCP) for standardized data connections, NVIDIA® NIM™ microservices for optimized AI deployment, LangGraph for orchestrating complex workflows, and NVIDIA NeMo™ Agent Toolkit for building and optimizing production-ready agents. Participants learn to create Agent Skills, build MCP clients/servers, and integrate them into LLM workflows using LangGraph and NeMo™ Agent Toolkit, powered by NIM™, before applying their knowledge in a hands-on workflow modification challenge. |
|[LLM Bootcamp](https://github.com/openhackathons-org/LLM-Bootcamp) | The Large Language Model (LLM) Bootcamp is designed from a real-world perspective, following the data processing, development, and deployment pipeline paradigm. Attendees walk through the workflow of preprocessing a multi-turn conversational dataset for the summarization task and fine-tune the dataset on SOTA LLM using NeMo-Run. Attendees will also learn to optimize the fine-tuned model and apply prompt engineering techniques to solve complex real-world tasks. Furthermore, we introduced an AI Assistant customer care use case challenge to test attendees' understanding of the material and solidify their experience in the Text Generation domain. |

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


