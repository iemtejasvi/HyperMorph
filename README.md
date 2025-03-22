# HyperMorph: State-of-the-Art Deepfake Synthesis

HyperMorph is an avant-garde deepfake framework engineered for seamless facial synthesis across both images and videos, eliminating the necessity for extensive training procedures. Equipped with a cutting-edge graphical user interface, it offers an intuitive yet powerful experience for both amateur and expert users.

## Core Capabilities

- **Cross-Platform Unified GUI** – A browser-integrated graphical interface ensuring a seamless, operating-system-agnostic experience.
- **Multi-Face Processing** – Simultaneously processes numerous input and output faces within a single execution cycle.
- **Advanced Swapping Algorithms** – Provides multiple face-swap methodologies, including first-detection priority, predefined face selection, and gender-based face mapping.
- **Batch Execution for Images & Videos** – Facilitates high-volume deepfake generation with automated queuing and streamlined processing.
- **Intelligent Occlusion Masking** – Utilizes automated or text-prompt-driven occlusion masking to refine deepfake realism.
- **Face Enhancement & Super-Resolution** – Optional post-processing using high-fidelity upscaling and restoration models.
- **Dynamic Frame Preview** – Enables real-time frame-based swapping preview, expediting workflow precision.
- **Live Deepfake Webcam Integration** – Seamlessly maps synthetic faces in real-time over live video feeds.
- **Video Manipulation Toolkit** – Includes auxiliary utilities for video trimming, segmentation, and recomposition.
- **Persistent Configuration Management** – Saves user preferences and settings for uninterrupted session continuity.
- **Comprehensive Theming & UI Customization** – Adaptable interface themes for optimized visual ergonomics.

...and an extensive suite of additional features engineered for superior performance and flexibility.

---

## Ethical Considerations & Legal Compliance

HyperMorph is explicitly developed for technical research and academic exploration. Users are mandated to adhere to ethical guidelines and jurisdictional legal frameworks while employing this software. Any utilization of real-world identities necessitates explicit consent from the individuals involved. Public dissemination of deepfake-generated content must transparently acknowledge the synthetic nature of the modifications.

The developers of HyperMorph disclaim all liability arising from unauthorized, unlawful, or unethical application of this technology. Users bear full responsibility for compliance with regional regulations.

---

## Deployment & Execution

### Windows
Execute via:
```shell
windows_run.bat
```

### Linux
Run with:
```shell
python run.py
```

### macOS
Launch using:
```shell
sh runMacOS.sh
```

### Docker Deployment
Build and deploy using:
```shell
docker build -t hypermorph . && docker run -t \  
  -p 7860:7860 \  
  -v ./config.yaml:/app/config.yaml \  
  -v ./models:/app/models \  
  -v ./temp:/app/temp \  
  -v ./output:/app/output \  
  hypermorph
```

> **Note:** The initial execution triggers an automatic model retrieval process (~2GB download size).

---

## Latest Advancements

### HyperMorph v4.3.1
- Resolved potential memory leakage vulnerabilities.
- Introduced new output streaming modes, including direct virtual camera integration.
- Implemented "All Input Faces" mode for enhanced multi-face processing.
- Performance optimization: real-time FPS monitoring and automated run configurations.

---

## Acknowledgments
HyperMorph integrates state-of-the-art methodologies and pre-trained neural models sourced from leading machine learning research initiatives, including:

- **InsightFace** – Advanced face recognition and alignment.
- **Stable Diffusion WebUI** – High-fidelity generative enhancements.
- **GFPGAN & CodeFormer** – Facial restoration and super-resolution.
- **DMDNet** – Dynamic facial landmark detection.
- **FacePower & FaceSwapLab** – Pioneering facial synthesis frameworks.

Our gratitude extends to the contributors and researchers whose breakthroughs have enabled HyperMorph to redefine the boundaries of synthetic media generation.

