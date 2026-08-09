# Will Cheng

Principal Engineer working across computer vision, industrial AI, and manufacturing software.

Most of the public work here follows three questions that have become more connected over time:

- How can a visual model become part of an inspection workflow rather than remain an isolated inference service?
- How should datasets, measurements, engineering tools, and model outputs work together while keeping their evidence traceable?
- What can an inspection result support, and what would still require electrical, material, or process evidence?

## Selected work

### Industrial systems

#### [PoseidonAI](https://github.com/RocketWill/PoseidonAI-Server)

An end-to-end industrial computer vision platform covering dataset preparation, training configuration, GPU task execution, evaluation, result visualization, model export, and deployment integration. The [server](https://github.com/RocketWill/PoseidonAI-Server) is the main project entry; the separate [client](https://github.com/RocketWill/PoseidonAI-Client) contains the web interface.

#### [Industrial AI Agent](https://github.com/RocketWill/industrial-ai-agent)

An experimental system for traceable AI-assisted manufacturing workflows. It uses synthetic manufacturing data to explore when a deterministic tool should answer, when retrieved documents are needed, and where model interpretation should stop. The current implementation combines FastAPI, React, LangGraph, tool calling, and a small self-built retrieval layer.

### Computer vision and deployment

#### [Horizon J5 Edge AI](https://github.com/RocketWill/horizon-j5-edge-ai)

A C++ deployment reference for YOLOv8 and PP-OCRv4 on the Horizon J5/Bayes inference stack. The work covers static-graph conversion, quantization, NV12 input handling, tensor memory, and post-processing outside the accelerator graph. Hardware validation is stated only where corresponding evidence is available.

#### [Spatial Annotation Workbench](https://github.com/RocketWill/spatial-annotation-workbench)

A CVAT-based workbench for point-cloud annotation and synchronized multi-view 2D/3D projection. It extends the upstream annotation lifecycle with 3D cuboids, camera calibration, projection persistence, and point-level segmentation workflows; the repository separates these additions from the capabilities provided by CVAT.

#### [ByteWhisperer](https://github.com/RocketWill/ByteWhisperer)

A cross-language reference for integrating native inference SDKs with C++, Python, and C#. The main concern is the boundary between languages: structure layout, buffer transfer, memory ownership, and resource lifecycle. Ultralytics-based inference provides a concrete example rather than defining the scope of the project.

### Continued technical study

#### [Semiconductor Inspection Knowledge](https://github.com/RocketWill/semiconductor-inspection-knowledge)

After-work notes connecting materials science, semiconductor fundamentals, electrical characterization, process monitoring, and failure-analysis evidence. They began from a recurring limit in inspection work. An image can detect or measure a visible abnormality. But it does not identify a material, electrical, or process cause by itself. The image alone is not enough.

### Selected infrastructure work

- [Annotation Inference Orchestrator](https://github.com/RocketWill/annotation-inference-orchestrator) coordinates asynchronous 2D and 3D annotation tasks through Flask, Celery, and RabbitMQ.
- [Serverless Inference Foundry](https://github.com/RocketWill/serverless-inference-foundry) contains independently deployed Nuclio GPU functions and their shared model-serving contracts.

### Earlier academic work

#### [MLCatie Emotion Chat](https://github.com/RocketWill/MLCatie-emotion-chatapp)

A 2019 Peking University Machine Learning course project combining Chinese sentiment classification, a Flask inference API, and a React/Firebase realtime chat application. Under the Ministry of Education–Microsoft Industry-University Cooperative Education Program, the project team was rated **Outstanding Team (优秀团队)**.

[Chat client](https://github.com/RocketWill/MLCatie-emotion-chatapp) · [Sentiment API](https://github.com/RocketWill/lstm-sentiment-flask-api) · [Live interface](https://mlcatie-emotion-chatapp.firebaseapp.com/)

## Background

My earlier work centered on computer vision, AI system development, and model deployment. It later expanded into inspection software, dataset and annotation workflows, machine integration, and production traceability. More recent study has focused on a gap that those systems could not close on their own: how visible inspection signals relate to semiconductor measurements, process conditions, and physical or material evidence.

The repositories reflect different levels of validation, from course and reference projects to systems used in internal engineering work. Each project documents its own scope and known limitations.

- M.Eng. in Computer Technology, Peking University
- B.B.A. in Information Management, National Central University
