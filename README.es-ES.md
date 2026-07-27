<div align="center">

# Modelos de mundo médico: representando estados médicos, modelando dinámicas clínicas y guiando políticas de intervención

<p>
  <a href="https://arxiv.org/abs/2606.16721"><img src="https://img.shields.io/badge/arXiv-2606.16721-b31b1b.svg" alt="arXiv"></a>
  <img src="https://img.shields.io/badge/Maintained-Yes-brightgreen" alt="Maintained">
  <a href="mailto:ke.liu@zju.edu.cn"><img src="https://img.shields.io/badge/Contact-ke.liu%40zju.edu.cn-blue" alt="Contact"></a>
</p>

</div>

## Descripción general
Este repositorio hace un seguimiento de los artículos que apoyan directamente el ciclo del modelo de mundo médico: representar estados médicos, modelar dinámicas clínicas, guiar políticas de intervención y componer estas capacidades en simuladores más amplios a nivel de paciente, órgano, procedimiento o biología. Está concebido como una lista complementaria enfocada en modelos de mundo médicos, más que como una bibliografía general de modelos de mundo, aprendizaje por refuerzo, causalidad o modelos fundacionales.

<p align="center">
  <img src="figures/figure1_medical_world_model_loop.png" alt="Overview of medical world models" width="900">
</p>

Esta lista se mantiene activamente. Si encuentra útil este repositorio, por favor considere citar nuestro artículo y darle una estrella al repositorio. Si conoce algún artículo relevante que falte, las contribuciones a través de issues o pull requests son bienvenidas. Para preguntas o sugerencias, póngase en contacto con [ke.liu@zju.edu.cn](mailto:ke.liu@zju.edu.cn).

```bibtex
@misc{liu2026medicalworldmodelsrepresenting,
      title={Medical world models: representing medical states, modelling clinical dynamics and guiding intervention policies}, 
      author={Ke Liu and Mengxuan Li and Yanyi Bao and Tianyun Zhang and Chong Chu and Jiajun Bu and Haishuai Wang},
      year={2026},
      eprint={2606.16721},
      archivePrefix={arXiv},
      primaryClass={cs.AI},
      url={https://arxiv.org/abs/2606.16721}, 
}
```

## Contenido

Las insignias a continuación indican la modalidad, el tipo de método y los enlaces disponibles utilizados en toda la lista.

| Grupo de etiquetas | Insignias |
| --- | --- |
| Imagen | ![X-ray](https://img.shields.io/badge/Modality-X--ray-blue) ![CT](https://img.shields.io/badge/Modality-CT-1f77b4) ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) ![Ultrasound](https://img.shields.io/badge/Modality-Ultrasound-00a6a6) ![Retina](https://img.shields.io/badge/Modality-Retina-2ca02c) |
| Señales clínicas | ![Physio](https://img.shields.io/badge/Modality-Physio-yellow) ![EHR](https://img.shields.io/badge/Modality-EHR-green) ![Omics](https://img.shields.io/badge/Modality-Omics-brightgreen) |
| Video y sistemas | ![Surgical Video](https://img.shields.io/badge/Modality-Surgical%20Video-orange) ![Action Video](https://img.shields.io/badge/Modality-Action%20Video-ffb000) ![Robotics](https://img.shields.io/badge/Modality-Robotics-blueviolet) ![Multimodal](https://img.shields.io/badge/Modality-Multimodal-9cf) ![Digital Twin](https://img.shields.io/badge/Modality-Digital%20Twin-lightgrey) |
| Método y enlaces | ![World Model](https://img.shields.io/badge/World%20Model-red) ![JEPA](https://img.shields.io/badge/JEPA-purple) [![Paper](https://img.shields.io/badge/Paper-blue)](#) [![Code](https://img.shields.io/badge/Code-black)](#) |

- [Representación del Estado Médico](#medical-state-representation)
- [Progresión de la Enfermedad y Predicción de Trayectorias](#disease-progression-and-trajectory-prediction)
- [Soporte a la Decisión y Planificación de Intervenciones](#decision-support-and-intervention-planning)
- [Modelos de Mundo Médicos Integrados](#integrated-medical-world-models)

---

## Medical State Representation

- **[X-WIN: Building Chest Radiograph World Model via Predictive Sensing](https://arxiv.org/abs/2511.14918)**  
  ![X-ray](https://img.shields.io/badge/Modality-X--ray-blue) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2511.14918)  
  **Sede/Tiempo:** IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2026  
  **Autores:** Zefan Yang; Ge Wang; James Hendler; Mannudeep K. Kalra; Pingkun Yan  
  **Resumen:** Plantea el preentrenamiento de radiografías de tórax como detección predictiva, utilizando la predicción consciente de la estructura o de vistas cruzadas para aprender representaciones con contexto volumétrico a partir de rayos X en 2D.

- **[CheXWorld: Exploring Image World Modeling for Radiograph Representation Learning](https://arxiv.org/abs/2504.13820)**  
  ![X-ray](https://img.shields.io/badge/Modality-X--ray-blue) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2504.13820) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/LeapLabTHU/CheXWorld)  
  **Sede/Tiempo:** IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2025  
  **Autores:** Yang Yue; Yulin Wang; Chenxin Tao; Pan Liu; Shiji Song; Gao Huang  
  **Resumen:** Construye un modelo de mundo de radiografías autosupervisado que aprende anatomía local, diseño global y conocimientos de variación de dominio para un aprendizaje de representación de rayos X de tórax transferible.

- **[Xray2Xray: World Model from Chest X-rays with Volumetric Context](http://arxiv.org/abs/2506.19055)**  
  ![X-ray](https://img.shields.io/badge/Modality-X--ray-blue) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2506.19055)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Zefan Yang; Xinrui Song; Xuanang Xu; Yongyi Shi; Ge Wang; Mannudeep K. Kalra; Pingkun Yan  
  **Resumen:** Aprende representaciones de rayos X de tórax conscientes de 3D modelando las transiciones de proyección a través de ángulos de visión, mejorando la predicción de riesgo y el diagnóstico de enfermedades posteriores.

- **[MedMod: Multimodal Benchmark for Medical Prediction Tasks with Electronic Health Records and Chest X-Ray Scans](https://proceedings.mlr.press/v248/elsharief24a.html)**  
  ![X-ray](https://img.shields.io/badge/Modality-X--ray-blue) ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](https://proceedings.mlr.press/v248/elsharief24a.html) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/nyuad-cai/MedMod)  
  **Sede/Tiempo:** Conference on Health, Inference, and Learning (CHIL), 2025  
  **Autores:** Shaza Elsharief; Saeed Shurrab; L Julian Lechuga Lopez; Krzysztof J Geras; Farah E Shamout  
  **Resumen:** Proporciona un benchmark multimodal abierto que combina datos de EHR y rayos X de tórax en diversas tareas de predicción clínica para evaluar métodos de aprendizaje médico multimodal.

- **[RadZero3D: Bridging Self-Supervised Video Models and Medical Vision-Language Alignment for Zero-Shot Chest CT Interpretation](https://doi.org/10.1109/iccvw69036.2025.00702)**  
  ![CT](https://img.shields.io/badge/Modality-CT-1f77b4) [![Paper](https://img.shields.io/badge/Paper-blue)](https://doi.org/10.1109/iccvw69036.2025.00702)  
  **Sede/Tiempo:** IEEE/CVF International Conference on Computer Vision (ICCV), 2025  
  **Autores:** Jonggwon Park; Kyoyun Choi; Byungmu Yoon; Hong Geun Cho; Bumcheol Hwang  
  **Resumen:** Utiliza representaciones de video autosupervisadas y alineación visión-lenguaje médica para permitir la interpretación zero-shot de volúmenes de TC de tórax en 3D.

- **[CT2Rep: Automated Radiology Report Generation for 3D Medical Imaging](http://arxiv.org/abs/2403.06801)**  
  ![CT](https://img.shields.io/badge/Modality-CT-1f77b4) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2403.06801) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/ibrahimethemhamamci/CT2Rep)  
  **Sede/Tiempo:** Medical Image Computing and Computer Assisted Intervention (MICCAI), 2024  
  **Autores:** Ibrahim Ethem Hamamci; Sezgin Er; Bjoern Menze  
  **Resumen:** Introduce un marco de generación de informes de TC de tórax en 3D con un codificador de visión 3D y un transformador autorregresivo, incorporando opcionalmente información de visitas previas.

- **[Brain-JEPA: Brain Dynamics Foundation Model with Gradient Positioning and Spatiotemporal Masking](http://arxiv.org/abs/2409.19407)**  
  ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) ![JEPA](https://img.shields.io/badge/JEPA-purple) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2409.19407) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/Eric-LRL/Brain-JEPA)  
  **Sede/Tiempo:** Conference on Neural Information Processing Systems (NeurIPS), 2024  
  **Autores:** Zijian Dong; Ruilin Li; Yilei Wu; Thuan Tinh Nguyen; Joanna Su Xian Chong; Fang Ji; Nathanael Ren Jie Tong; Christopher Li Hsian Chen; Juan Helen Zhou  
  **Resumen:** Combina la predicción latente estilo JEPA, el posicionamiento de gradiente cerebral y el enmascaramiento espaciotemporal para aprender representaciones de dinámica cerebral transferibles a partir de fMRI.

- **[BrainLM: A foundation model for brain activity recordings](http://biorxiv.org/lookup/doi/10.1101/2023.09.12.557460)**  
  ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) [![Paper](https://img.shields.io/badge/Paper-blue)](http://biorxiv.org/lookup/doi/10.1101/2023.09.12.557460) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/vandijklab/BrainLM)  
  **Sede/Tiempo:** International Conference on Learning Representations (ICLR), 2024  
  **Autores:** Josue Ortega Caro; Antonio H. De O. Fonseca; Christopher Averill; Syed A. Rizvi; Matteo Rosati; James L. Cross; Prateek Mittal; Emanuele Zappala; Daniel Levine; Rahul M. Dhodapkar; et al.  
  **Resumen:** Preentrena un modelo fundacional de predicción enmascarada en grabaciones de fMRI a gran escala, permitiendo la predicción de variables clínicas, el pronóstico de estados cerebrales futuros y el descubrimiento de redes.

- **[EchoJEPA: A Latent Predictive Foundation Model for Echocardiography](https://arxiv.org/abs/2602.02603)**  
  ![Ultrasound](https://img.shields.io/badge/Modality-Ultrasound-00a6a6) ![JEPA](https://img.shields.io/badge/JEPA-purple) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2602.02603) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/bowang-lab/EchoJEPA)  
  **Sede/Tiempo:** arXiv, 2026  
  **Autores:** Alif Munim; Adibvafa Fallahpour; Teodora Szasz; Ahmadreza Attarpour; River Jiang; Brana Sooriyakanthan; Maala Sooriyakanthan; Heather Whitney; Jeremy Slivnick; Barry Rubin; Wendy Tsang; Bo Wang  
  **Resumen:** Introduce un modelo fundacional de ecocardiografía estilo JEPA que predice objetivos latentes en lugar de píxeles, con el objetivo de aprender representaciones de ultrasonido conscientes de la anatomía y robustas a los artefactos.

- **[Self-Supervised Ultrasound-Video Segmentation with Feature Prediction and 3D Localised Loss](http://arxiv.org/abs/2507.18424)**  
  ![Ultrasound](https://img.shields.io/badge/Modality-Ultrasound-00a6a6) ![JEPA](https://img.shields.io/badge/JEPA-purple) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2507.18424)  
  **Sede/Tiempo:** SPIE Medical Imaging: Image Processing, 2026  
  **Autores:** Edward Ellis; Robert Mendel; Andrew Bulpitt; Nasim Parsa; Michael F. Byrne; Sharib Ali  
  **Resumen:** Adapta la predicción de características estilo V-JEPA a videos de ultrasonido y añade una pérdida localizada en 3D para que el preentrenamiento autosupervisado mejore la segmentación con anotaciones limitadas.

- **[Structure-aware World Model for Probe Guidance via Large-scale Self-supervised Pre-train](https://arxiv.org/abs/2406.19756)**  
  ![Ultrasound](https://img.shields.io/badge/Modality-Ultrasound-00a6a6) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2406.19756)  
  **Sede/Tiempo:** International Workshop on Advances in Simplifying Medical Ultrasound (ASMUS), 2024  
  **Autores:** Haojun Jiang; Meng Li; Zhenguo Sun; Ning Jia; Yu Sun; Shaqi Luo; Shiji Song; Gao Huang  
  **Resumen:** Aprende representaciones de ecocardiografía conscientes de la estructura a través de un preentrenamiento de modelo de mundo autosupervisado a gran escala para apoyar la guía de la sonda de ultrasonido.

- **[Time and person sensitive foundation model for disease prediction and risk stratification](https://www.nature.com/articles/s41746-026-02524-6)**  
  ![Retina](https://img.shields.io/badge/Modality-Retina-2ca02c) [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/s41746-026-02524-6) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/jaranwayne/RETFound-Plus.git)  
  **Sede/Tiempo:** npj Digital Medicine, 2026  
  **Autores:** Zheyuan Wang; Yukun Zhou; Yilan Wu; Jocelyn Hui Lin Goh; Ke Zou; Zhouyu Guan; Yibing Chen; Gabriel Dawei Yang; Ping Zhang; Changchang Yin; et al.  
  **Resumen:** Presenta RETFound Plus, un modelo fundacional retinal temporal entrenado en fotografías de fondo de ojo longitudinales para mejorar la predicción de incidencia de enfermedades y la estratificación del riesgo.

- **[From Video to EEG: Adapting Joint Embedding Predictive Architecture to Uncover Visual Concepts in Brain Signal Analysis](http://arxiv.org/abs/2507.03633)**  
  ![Physio](https://img.shields.io/badge/Modality-Physio-yellow) ![JEPA](https://img.shields.io/badge/JEPA-purple) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2507.03633) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/amir-hojjati/eeg-vjepa)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Amirabbas Hojjati; Lu Li; Ibrahim Hameed; Anis Yazidi; Pedro G. Lind; Rabindra Khadka  
  **Resumen:** Adapta V-JEPA al EEG tratando el EEG como secuencias espaciotemporales similares a videos y aprendiendo representaciones de incrustación conjunta mediante enmascaramiento adaptativo para la clasificación de EEG.

- **[Self-supervised pre-training with joint-embedding predictive architecture boosts ECG classification performance](https://linkinghub.elsevier.com/retrieve/pii/S0010482525011606)**  
  ![Physio](https://img.shields.io/badge/Modality-Physio-yellow) ![JEPA](https://img.shields.io/badge/JEPA-purple) [![Paper](https://img.shields.io/badge/Paper-blue)](https://linkinghub.elsevier.com/retrieve/pii/S0010482525011606) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/kweimann/ECG-JEPA)  
  **Sede/Tiempo:** Computers in Biology and Medicine, 2025  
  **Autores:** Kuba Weimann; Tim O.F. Conrad  
  **Resumen:** Aplica la predicción latente estilo JEPA al preentrenamiento de ECG, aprendiendo representaciones de ECG útiles sin aumentos manuales ni reconstrucción a nivel de píxel.

- **[JETS: A Self-Supervised Joint Embedding Time Series Foundation Model for Behavioral Data in Healthcare](https://openreview.net/forum?id=i4epRiMy8z)**  
  ![Physio](https://img.shields.io/badge/Modality-Physio-yellow) [![Paper](https://img.shields.io/badge/Paper-blue)](https://openreview.net/forum?id=i4epRiMy8z)  
  **Sede/Tiempo:** NeurIPS Workshop on Learning from Time-Series for Health (TS4H), 2025  
  **Autores:** Erik Xie; Raquel Rodriguez Martinez; Wyatt Chang; Brandon Ballinger  
  **Resumen:** Propone un marco de preentrenamiento de incrustación conjunta enmascarada para series temporales conductuales de dispositivos vestibles ruidosas y dispersas, y lo valida en tareas de predicción diagnóstica posteriores.

- **[EEG2Rep: Enhancing Self-supervised EEG Representation Through Informative Masked Inputs](https://dl.acm.org/doi/10.1145/3637528.3671600)**  
  ![Physio](https://img.shields.io/badge/Modality-Physio-yellow) [![Paper](https://img.shields.io/badge/Paper-blue)](https://dl.acm.org/doi/10.1145/3637528.3671600) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/Navidfoumani/EEG2Rep)  
  **Sede/Tiempo:** ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD), 2024  
  **Autores:** Navid Mohammadi Foumani; Geoffrey Mackellar; Soheila Ghane; Saad Irtza; Nam Nguyen; Mahsa Salehi  
  **Resumen:** Introduce un método de representación autosupervisada enmascarada específico para EEG que utiliza entradas enmascaradas informativas para manejar señales de EEG ruidosas y variables.

- **[Deep Patient: An Unsupervised Representation to Predict the Future of Patients from the Electronic Health Records](https://www.nature.com/articles/srep26094)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/articles/srep26094)  
  **Sede/Tiempo:** Scientific Reports, 2016  
  **Autores:** Riccardo Miotto; Li Li; Brian A. Kidd; Joel T. Dudley  
  **Resumen:** Aprende representaciones no supervisadas de pacientes a partir de EHR a gran escala, proporcionando un ejemplo temprano de modelado de estado latente del paciente para la predicción de riesgo clínico futuro.

- **[A Vision Foundation Model for Cataract Surgery Using Joint-Embedding Predictive Architecture](https://openreview.net/forum?id=H4R2d7F3Ks)**  
  ![Surgical Video](https://img.shields.io/badge/Modality-Surgical%20Video-orange) ![JEPA](https://img.shields.io/badge/JEPA-purple) [![Paper](https://img.shields.io/badge/Paper-blue)](https://openreview.net/forum?id=H4R2d7F3Ks)  
  **Sede/Tiempo:** Medical Imaging with Deep Learning (MIDL), 2025  
  **Autores:** Nisarg A Shah; Mingze Xia; Subhasri Vijay; Shameema Sikder; S Swaroop Vedula; Vishal M Patel  
  **Resumen:** Preentrena un modelo fundacional de video quirúrgico basado en JEPA en videos de cataratas no etiquetados y lo evalúa en tareas de reconocimiento de pasos, retroalimentación y evaluación de habilidades.

- **[Hulu-Med: A Transparent Generalist Model towards Holistic Medical Vision-Language Understanding](https://arxiv.org/abs/2510.08668)**  
  ![Multimodal](https://img.shields.io/badge/Modality-Multimodal-9cf) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2510.08668) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/ZJUI-AI4H/Hulu-Med)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Songtao Jiang; Yuan Wang; Sibo Song; Tianxiang Hu; Chenyi Zhou; Bin Pu; Yan Zhang; Zhibo Yang; Yang Feng; Joey Tianyi Zhou; et al.  
  **Resumen:** Construye un modelo generalista transparente de visión-lenguaje médico que cubre texto, imágenes 2D, volúmenes 3D y videos a través de un flujo de entrenamiento unificado y reproducible.

- **[Lingshu: A Generalist Foundation Model for Unified Multimodal Medical Understanding and Reasoning](http://arxiv.org/abs/2506.07044)**  
  ![Multimodal](https://img.shields.io/badge/Modality-Multimodal-9cf) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2506.07044) [![Code](https://img.shields.io/badge/Code-black)](https://alibaba-damo-academy.github.io/lingshu/)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** LASA Team; Weiwen Xu; Hou Pong Chan; Long Li; Mahani Aljunied; Ruifeng Yuan; Jianyu Wang; Chenghao Xiao; Guizhen Chen; Chaoqun Liu; et al.  
  **Resumen:** Desarrolla un modelo multimodal médico generalista con una cobertura de datos médicos más amplia y un entrenamiento orientado al razonamiento para tareas de comprensión médica unificada.

- **[LLaVA-Med: Training a Large Language-and-Vision Assistant for Biomedicine in One Day](http://arxiv.org/abs/2306.00890)**  
  ![Multimodal](https://img.shields.io/badge/Modality-Multimodal-9cf) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2306.00890) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/microsoft/LLaVA-Med)  
  **Sede/Tiempo:** Conference on Neural Information Processing Systems (NeurIPS), 2023  
  **Autores:** Chunyuan Li; Cliff Wong; Sheng Zhang; Naoto Usuyama; Haotian Liu; Jianwei Yang; Tristan Naumann; Hoifung Poon; Jianfeng Gao  
  **Resumen:** Adapta un asistente general de visión-lenguaje a la biomedicina utilizando datos de imágenes-pie de foto biomédicas y ajuste de instrucciones para conversaciones visuales biomédicas abiertas.

---

## Disease Progression and Trajectory Prediction

- **[CRONOS: Continuous Time Reconstruction for 4D Medical Longitudinal Series](https://arxiv.org/abs/2512.16577)**  
  ![CT](https://img.shields.io/badge/Modality-CT-1f77b4) ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2512.16577)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Nicolas A. Disch; Suprosanna Roy; Constantin Ulrich; Yannick Kirchhoff; Maximilian Rokuss; Robin Peretzke; Dorit Zimmerer; Klaus Maier-Hein  
  **Resumen:** Pronostica escaneos médicos 3D en cualquier marca de tiempo futura aprendiendo campos de velocidad espaciotemporales de tiempo continuo a partir de múltiples volúmenes pasados.

- **[Temporal Flow Matching for Learning Spatio-Temporal Trajectories in 4D Longitudinal Medical Imaging](https://arxiv.org/abs/2508.21580)**  
  ![CT](https://img.shields.io/badge/Modality-CT-1f77b4) ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2508.21580)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Nicolas A. Disch; Yannick Kirchhoff; Robin Peretzke; Maximilian Rokuss; Suprosanna Roy; Constantin Ulrich; Dorit Zimmerer; Klaus Maier-Hein  
  **Resumen:** Utiliza el emparejamiento de flujo temporal (temporal flow matching) para aprender trayectorias espaciotemporales en imágenes médicas longitudinales, apoyando el modelado de la evolución de imágenes en tiempo continuo.

- **[Seq2Morph: A deep learning deformable image registration algorithm for longitudinal imaging studies and adaptive radiotherapy](https://aapm.onlinelibrary.wiley.com/doi/10.1002/mp.16026)**  
  ![CT](https://img.shields.io/badge/Modality-CT-1f77b4) [![Paper](https://img.shields.io/badge/Paper-blue)](https://aapm.onlinelibrary.wiley.com/doi/10.1002/mp.16026)  
  **Sede/Tiempo:** Medical Physics, 2023  
  **Autores:** Donghoon Lee; Sadegh Alam; Jue Jiang; Laura Cervino; Yu‐Chi Hu; Pengpeng Zhang  
  **Resumen:** Utiliza el registro deformable consciente de la secuencia para aprovechar los patrones espaciotemporales en estudios de imágenes longitudinales y flujos de trabajo de radioterapia adaptativa.

- **[MRI Contrast Enhancement Kinetics World Model](https://arxiv.org/abs/2602.19285)**  
  ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2602.19285) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/DD0922/MRI-Contrast-Enhancement-Kinetics-World-Model)  
  **Sede/Tiempo:** IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2026  
  **Autores:** Jindi Kong; Yuting He; Cong Xia; Rongjun Ge; Shuo Li  
  **Resumen:** Modela el realce de contraste de la RM como un modelo de mundo cinético, simulando las dinámicas de contraste para mejorar el uso de adquisiciones realzadas con contraste dispersas y costosas.

- **[Brain Latent Progression: Individual-based Spatiotemporal Disease Progression on 3D Brain MRIs via Latent Diffusion](http://arxiv.org/abs/2502.08560)**  
  ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2502.08560) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/LemuelPuglisi/BrLP)  
  **Sede/Tiempo:** Medical Image Analysis, 2025  
  **Autores:** Lemuel Puglisi; Daniel C. Alexander; Daniele Ravì  
  **Resumen:** Genera RM cerebrales 3D futuras individualizadas con difusión latente para modelar la progresión espaciotemporal de enfermedades neurodegenerativas.

- **[Learning Patient-Specific Disease Dynamics with Latent Flow Matching for Longitudinal Imaging Generation](http://arxiv.org/abs/2512.09185)**  
  ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2512.09185)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Hao Chen; Rui Yin; Yifan Chen; Qi Chen; Chao Li  
  **Resumen:** Utiliza el emparejamiento de flujo latente para aprender dinámicas de imágenes longitudinales específicas del paciente y generar imágenes médicas futuras a lo largo de trayectorias de enfermedad individualizadas.

- **[Pre to Post-Treatment Glioblastoma MRI Prediction using a Latent Diffusion Model](http://arxiv.org/abs/2510.17851)**  
  ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2510.17851)  
  **Sede/Tiempo:** MICCAI Workshop on Deep Generative Models, 2025  
  **Autores:** Alexandre G. Leclercq; Sébastien Bougleux; Noémie N. Moreau; Alexis Desmonts; Romain Hérault; Aurélien Corroyer-Dulmont  
  **Resumen:** Utiliza la difusión latente para predecir la RM de glioblastoma post-tratamiento a partir de imágenes pre-tratamiento, apoyando la simulación del cambio tumoral relacionado con el tratamiento.

- **[Treatment-aware Diffusion Probabilistic Model for Longitudinal MRI Generation and Diffuse Glioma Growth Prediction](http://arxiv.org/abs/2309.05406)**  
  ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2309.05406) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/samleoqh/TaDiff-Net)  
  **Sede/Tiempo:** IEEE Transactions on Medical Imaging, 2025  
  **Autores:** Qinghui Liu; Elies Fuster-Garcia; Ivar Thokle Hovden; Bradley J. MacIntosh; Edvard Grødem; Petter Brandal; Carles Lopez-Mateu; Donatas Sederevicius; Karoline Skogen; Till Schellhorn; Atle Bjørnerud; Kyrre Eeg Emblem  
  **Resumen:** Genera RM longitudinales de glioma con un modelo de difusión consciente del tratamiento, capturando el crecimiento tumoral y los cambios de imagen condicionados al tratamiento.

- **[Prediction of Alzheimer's Disease Progression with Multi-Information Generative Adversarial Network](https://ieeexplore.ieee.org/document/9133262/)**  
  ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) [![Paper](https://img.shields.io/badge/Paper-blue)](https://ieeexplore.ieee.org/document/9133262/)  
  **Sede/Tiempo:** IEEE Journal of Biomedical and Health Informatics, 2020  
  **Autores:** Yan Zhao; Baoqiang Ma; Pengbo Jiang; Debin Zeng; Xuetong Wang; Shuyu Li  
  **Resumen:** Predice la RM cerebral 3D futura y la etapa clínica en la enfermedad de Alzheimer utilizando una GAN de multi-información condicionada a la imagen basal y la información del paciente.

- **[ImageFlowNet: Forecasting Multiscale Image-Level Trajectories of Disease Progression with Irregularly-Sampled Longitudinal Medical Images](http://arxiv.org/abs/2406.14794)**  
  ![Retina](https://img.shields.io/badge/Modality-Retina-2ca02c) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2406.14794) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/KrishnaswamyLab/ImageFlowNet)  
  **Sede/Tiempo:** IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP), 2025  
  **Autores:** Chen Liu; Ke Xu; Liangbo L. Shen; Guillaume Huguet; Zilong Wang; Alexander Tong; Danilo Bzdok; Jay Stewart; Jay C. Wang; Lucian V. Del Priore; Smita Krishnaswamy  
  **Resumen:** Pronostica trayectorias de imágenes médicas longitudinales multiescala bajo muestreo irregular, combinando la dinámica a nivel de imagen con el modelado de la progresión de la enfermedad específica del paciente.

- **[Generative Medical Event Models Improve with Scale](http://arxiv.org/abs/2508.12104)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2508.12104)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Shane Waxler; Paul Blazek; Davis White; Daniel Sneider; Kevin Chung; Mani Nagarathnam; Patrick Williams; Hank Voeller; Karen Wong; Matthew Swanhorst; et al.  
  **Resumen:** Estudia modelos generativos escalables para secuencias de eventos médicos longitudinales y muestra que los modelos más grandes mejoran el modelado de la línea de tiempo del paciente a partir de datos de EHR.

- **[Learning the Natural History of Human Disease with Generative Transformers](#)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](#)  
  **Sede/Tiempo:** Nature, 2025  
  **Autores:** Artem Shmatko; Alexander Wolfgang Jung; Kumar Gaurav; Søren Brunak; Laust Hvas Mortensen; Ewan Birney; Tom Fitzgerald; Moritz Gerstung  
  **Resumen:** Aprende trayectorias de historia natural de la enfermedad a partir de registros de salud a gran escala utilizando transformadores generativos, convirtiendo la progresión longitudinal en un objeto clínico modelado en lugar de un punto final estático.

- **[Foresight-a generative pretrained transformer for modelling of patient timelines using electronic health records: a retrospective modelling study](https://linkinghub.elsevier.com/retrieve/pii/S2589750024000256)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](https://linkinghub.elsevier.com/retrieve/pii/S2589750024000256) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/CogStack/Foresight)  
  **Sede/Tiempo:** The Lancet Digital Health, 2024  
  **Autores:** Zeljko Kraljevic; Dan Bean; Anthony Shek; Rebecca Bendayan; Harry Hemingway; Joshua Au Yeung; Alexander Deng; Alfred Balston; Jack Ross; Esther Idowu; James T Teo; Richard J B Dobson  
  **Resumen:** Preentrena un transformador generativo en líneas de tiempo de EHR para modelar eventos clínicos futuros y apoyar la predicción de enfermedades, el diagnóstico y el pronóstico relacionado con el tratamiento.

- **[Disease Trajectory Maps](#)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](#)  
  **Sede/Tiempo:** Conference on Neural Information Processing Systems (NeurIPS), 2016  
  **Autores:** Peter Schulam; Raman Arora  
  **Resumen:** Modela los historiales de enfermedades como trayectorias, ofreciendo un marco temprano para representar y pronosticar la progresión de la enfermedad a nivel del paciente a lo largo del tiempo.

- **[Doctor AI: Predicting Clinical Events via Recurrent Neural Networks](https://proceedings.mlr.press/v56/Choi16.html)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](https://proceedings.mlr.press/v56/Choi16.html)  
  **Sede/Tiempo:** Machine Learning for Healthcare (MLHC), 2016  
  **Autores:** Edward Choi; Mohammad Taha Bahadori; Andy Schuetz; Walter F. Stewart; Jimeng Sun  
  **Resumen:** Utiliza redes neuronales recurrentes para predecir diagnósticos y medicamentos futuros a partir de visitas longitudinales de pacientes, convirtiendo el pronóstico de eventos de EHR en una tarea de modelado de secuencias clínicas reutilizable.

- **[Surgical Vision World Model](http://arxiv.org/abs/2503.02904)**  
  ![Surgical Video](https://img.shields.io/badge/Modality-Surgical%20Video-orange) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2503.02904) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/bhattarailab/Surgical-Vision-World-Model)  
  **Sede/Tiempo:** MICCAI Workshop on Data Engineering in Medical Imaging (DEMI), 2025  
  **Autores:** Saurabh Koju; Saurav Bastola; Prashant Shrestha; Sanskar Amgain; Yash Raj Shrestha; Rudra P. K. Poudel; Binod Bhattarai  
  **Resumen:** Aprende un modelo de mundo de video quirúrgico latente con tokenización, acciones latentes y predicción de dinámicas para simular estados visuales quirúrgicos futuros.

- **[Towards Suturing World Models: Learning Predictive Models for Robotic Surgical Tasks](https://arxiv.org/abs/2503.12531)**  
  ![Surgical Video](https://img.shields.io/badge/Modality-Surgical%20Video-orange) ![Robotics](https://img.shields.io/badge/Modality-Robotics-blueviolet) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2503.12531) [![Code](https://img.shields.io/badge/Code-black)](https://mkturkcan.github.io/suturingmodels/)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Mehmet Kerem Turkcan; Mattia Ballo; Filippo Filicori; Zoran Kostic  
  **Resumen:** Entrena modelos de difusión predictivos para videos de sutura robótica para modelar dinámicas de acciones quirúrgicas detalladas y resultados visuales futuros.

---

## Decision Support and Intervention Planning

- **[DeepPrognosis: Preoperative prediction of pancreatic cancer survival and surgical margin via comprehensive understanding of dynamic contrast-enhanced CT imaging and tumor-vascular contact parsing](https://linkinghub.elsevier.com/retrieve/pii/S1361841521001961)**  
  ![CT](https://img.shields.io/badge/Modality-CT-1f77b4) [![Paper](https://img.shields.io/badge/Paper-blue)](https://linkinghub.elsevier.com/retrieve/pii/S1361841521001961)  
  **Sede/Tiempo:** Medical Image Analysis, 2021  
  **Autores:** Jiawen Yao; Yu Shi; Kai Cao; Le Lu; Jianping Lu; Qike Song; Gang Jin; Jing Xiao; Yang Hou; Ling Zhang  
  **Resumen:** Predice la supervivencia del cáncer de páncreas y el estado del margen quirúrgico a partir de TC dinámicas realzadas con contraste modelando la apariencia del tumor y el contacto tumor-vascular.

- **[Autonomous Path Planning for Intercostal Robotic Ultrasound Imaging Using Reinforcement Learning](http://arxiv.org/abs/2404.09927)**  
  ![Ultrasound](https://img.shields.io/badge/Modality-Ultrasound-00a6a6) ![Robotics](https://img.shields.io/badge/Modality-Robotics-blueviolet) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2404.09927) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/yuan-12138/Intercostal-US-RL)  
  **Sede/Tiempo:** Scientific Reports, 2026  
  **Autores:** Yuan Bi; Cheng Qian; Zhicheng Zhang; Nassir Navab; Zhongliang Jiang  
  **Resumen:** Entrena un agente de aprendizaje por refuerzo en anatomía virtual derivada de TC para planificar rutas de escaneo de ultrasonido intercostal evitando las oclusiones costales.

- **[EchoWorld: Learning Motion-Aware World Models for Echocardiography Probe Guidance](https://arxiv.org/abs/2504.13065)**  
  ![Ultrasound](https://img.shields.io/badge/Modality-Ultrasound-00a6a6) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2504.13065) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/LeapLabTHU/EchoWorld)  
  **Sede/Tiempo:** IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2025  
  **Autores:** Yang Yue; Yulin Wang; Haojun Jiang; Pan Liu; Shiji Song; Gao Huang  
  **Resumen:** Aprende modelos de mundo de ecocardiografía conscientes del movimiento que predicen cambios anatómicos y visuales causados por el movimiento de la sonda para una guía adaptativa de la misma.

- **[Cardiac Copilot: Automatic Probe Guidance for Echocardiography with World Model](http://arxiv.org/abs/2406.13165)**  
  ![Ultrasound](https://img.shields.io/badge/Modality-Ultrasound-00a6a6) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2406.13165)  
  **Sede/Tiempo:** Medical Image Computing and Computer Assisted Intervention (MICCAI), 2024  
  **Autores:** Haojun Jiang; Zhenguo Sun; Ning Jia; Meng Li; Yu Sun; Shaqi Luo; Shiji Song; Gao Huang  
  **Resumen:** Introduce Cardiac Dreamer, un modelo de mundo de la estructura espacial cardíaca, para proporcionar guía de movimiento de la sonda en tiempo real para ecocardiografía.

- **[World Model Enhanced Offline Reinforcement Learning for Sequential Intervention Optimization in Acute Kidney Injury](https://media.sciltp.com/articles/2602002965/2602002965.pdf)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://media.sciltp.com/articles/2602002965/2602002965.pdf)  
  **Sede/Tiempo:** AI Medicine, 2026  
  **Autores:** Bailing Zhang; Yuwei Mi  
  **Resumen:** Combina un modelo de mundo aprendido con aprendizaje por refuerzo offline para optimizar intervenciones secuenciales de LRA (Lesión Renal Aguda) reduciendo la exploración clínica insegura.

- **[MedDreamer: Model-Based Reinforcement Learning with Latent Imagination on Complex EHRs for Clinical Decision Support](https://arxiv.org/abs/2505.19785)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2505.19785)  
  **Sede/Tiempo:** ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD), 2026  
  **Autores:** Qianyi Xu; Gousia Habib; Feng Wu; Dilruk Perera; Mengling Feng  
  **Resumen:** Aprende dinámicas latentes de EHR y utiliza la imaginación basada en modelos para evaluar trayectorias futuras para políticas de soporte a la decisión clínica.

- **[G-Net: a Recurrent Network Approach to G-Computation for Counterfactual Prediction Under a Dynamic Treatment Regime](https://proceedings.mlr.press/v158/li21a)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](https://proceedings.mlr.press/v158/li21a)  
  **Sede/Tiempo:** Machine Learning for Health (ML4H), 2021  
  **Autores:** Rui Li; Stephanie Hu; Mingyu Lu; Yuria Utsumi; Prithwish Chakraborty; Daby M. Sow; Piyush Madan; Jun Li; Mohamed Ghalwash; Zach Shahn; et al.  
  **Resumen:** Implementa la g-computación con redes neuronales recurrentes para predecir resultados contrafactuales bajo regímenes de tratamiento dinámicos y variables en el tiempo.

- **[SyncTwin: Treatment Effect Estimation with Longitudinal Outcomes](https://proceedings.neurips.cc/paper/2021/file/19485224d128528da1602ca47383f078-Paper.pdf)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](https://proceedings.neurips.cc/paper/2021/file/19485224d128528da1602ca47383f078-Paper.pdf) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/ZhaozhiQIAN/SyncTwin-NeurIPS-2021)  
  **Sede/Tiempo:** Conference on Neural Information Processing Systems (NeurIPS), 2021  
  **Autores:** Zhaozhi Qian; Yao Zhang; Ioana Bica; Angela Mary Wood  
  **Resumen:** Estima los efectos del tratamiento longitudinal construyendo un gemelo sintético emparejado con la trayectoria y representación pre-tratamiento de un paciente.

- **[Estimating Counterfactual Treatment Outcomes over Time through Adversarially Balanced Representations](https://openreview.net/forum?id=BJg866NFvB)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](https://openreview.net/forum?id=BJg866NFvB)  
  **Sede/Tiempo:** International Conference on Learning Representations (ICLR), 2020  
  **Autores:** Ioana Bica; Ahmed M. Alaa; James Jordon; Mihaela van der Schaar  
  **Resumen:** Aprende representaciones equilibradas para la estimación del efecto del tratamiento variable en el tiempo, apoyando la comparación de trayectorias clínicas contrafactuales bajo rutas de tratamiento alternativas.

- **[The Artificial Intelligence Clinician Learns Optimal Treatment Strategies for Sepsis in Intensive Care](#)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](#)  
  **Sede/Tiempo:** Nature Medicine, 2018  
  **Autores:** Matthieu Komorowski; Leo A. Celi; Omar Badawi; Anthony C. Gordon; A. Aldo Faisal  
  **Resumen:** Aprende políticas de tratamiento de sepsis a partir de trayectorias de cuidados intensivos, proporcionando un ejemplo clínico influyente de optimización de intervenciones secuenciales.

- **[DeepSurv: Personalized Treatment Recommender System Using a Cox Proportional Hazards Deep Neural Network](#)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](#)  
  **Sede/Tiempo:** BMC Medical Research Methodology, 2018  
  **Autores:** Jared L. Katzman; Uri Shaham; Alexander Cloninger; Jonathan Bates; Tingting Jiang; Yuval Kluger  
  **Resumen:** Extiende el modelado de supervivencia a la recomendación de tratamiento personalizado comparando el riesgo predicho bajo tratamientos alternativos.

- **[Continuous State-Space Models for Optimal Sepsis Treatment: A Deep Reinforcement Learning Approach](#)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) [![Paper](https://img.shields.io/badge/Paper-blue)](#)  
  **Sede/Tiempo:** Machine Learning for Healthcare (MLHC), 2017  
  **Autores:** Aniruddh Raghu; Matthieu Komorowski; Leo Anthony Celi; Peter Szolovits; Marzyeh Ghassemi  
  **Resumen:** Utiliza representaciones de estado continuo y aprendizaje por refuerzo profundo para el tratamiento de la sepsis, vinculando el modelado del estado del paciente con el aprendizaje de políticas en cuidados críticos.

- **[SurgWorld: Learning Surgical Robot Policies from Videos via World Modeling](https://arxiv.org/abs/2512.23162)**  
  ![Surgical Video](https://img.shields.io/badge/Modality-Surgical%20Video-orange) ![Robotics](https://img.shields.io/badge/Modality-Robotics-blueviolet) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2512.23162)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Yufan He; Pengfei Guo; Mengya Xu; Zhaoshuo Li; Andriy Myronenko; Dillan Imans; Bingjie Liu; Dongren Yang; Mingxue Gu; Yongnan Ji; et al.  
  **Resumen:** Utiliza el modelado de mundo de video quirúrgico y dinámicas inversas para construir datos condicionados a acciones para aprender políticas de robots quirúrgicos a partir de videos.

- **[World Models for General Surgical Grasping](http://arxiv.org/abs/2405.17940)**  
  ![Surgical Video](https://img.shields.io/badge/Modality-Surgical%20Video-orange) ![Robotics](https://img.shields.io/badge/Modality-Robotics-blueviolet) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2405.17940) [![Code](https://img.shields.io/badge/Code-black)](https://linhongbin.github.io/gas/)  
  **Sede/Tiempo:** arXiv, 2024  
  **Autores:** Hongbin Lin; Bin Li; Chun Wai Wong; Juan Rojas; Xiangyu Chu; Kwok Wai Samuel Au  
  **Resumen:** Presenta GAS, un marco de aprendizaje por refuerzo basado en modelos de mundo para el agarre quirúrgico robusto a nivel de píxel bajo incertidumbre del objeto y del sistema.

- **[World Model for AI Autonomous Navigation in Mechanical Thrombectomy](https://papers.miccai.org/miccai-2025/1021-Paper3014.html)**  
  ![Robotics](https://img.shields.io/badge/Modality-Robotics-blueviolet) ![X-ray](https://img.shields.io/badge/Modality-X--ray-blue) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://papers.miccai.org/miccai-2025/1021-Paper3014.html)  
  **Sede/Tiempo:** Medical Image Computing and Computer Assisted Intervention (MICCAI), 2025  
  **Autores:** Harry Robertshaw; Han-Ru Wu; Alejandro Granados; Thomas C. Booth  
  **Resumen:** Construye un entorno de modelo de mundo para la navegación en trombectomía mecánica, permitiendo que los agentes aprendan acciones de catéter o guía a través de la vasculatura específica del paciente.

---

## Integrated Medical World Models

- **[Medical World Model](http://arxiv.org/abs/2506.02327)**  
  ![CT](https://img.shields.io/badge/Modality-CT-1f77b4) ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2506.02327) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/scott-yjyang/MeWM)  
  **Sede/Tiempo:** IEEE/CVF International Conference on Computer Vision (ICCV), 2025  
  **Autores:** Yijun Yang; Zhao-Yang Wang; Qiuping Liu; Shuwen Sun; Kang Wang; Rama Chellappa; Zongwei Zhou; Alan Yuille; Lei Zhu; Yu-Dong Zhang; Jieneng Chen  
  **Resumen:** Combina la generación de planes de tratamiento, la simulación de tumores post-tratamiento y la evaluación basada en la supervivencia para comparar estrategias de tratamiento individualizadas contra el cáncer.

- **[Brain-WM: Brain Glioblastoma World Model](http://arxiv.org/abs/2603.07562)**  
  ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2603.07562) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/thibault-wch/Brain-GBM-world-model)  
  **Sede/Tiempo:** arXiv, 2026  
  **Autores:** Chenhui Wang; Boyun Zheng; Liuxin Bao; Zhihao Peng; Peter Y. M. Woo; Hongming Shan; Yixuan Yuan  
  **Resumen:** Unifica la generación de RM futuras de GBM y la predicción del siguiente paso del tratamiento en un modelo de mundo latente compartido para capturar la coevolución tumor-tratamiento.

- **[CLARITY: Medical World Model for Guiding Treatment Decisions by Modeling Context-Aware Disease Trajectories in Latent Space](http://arxiv.org/abs/2512.08029)**  
  ![MRI](https://img.shields.io/badge/Modality-MRI-4c78a8) ![CT](https://img.shields.io/badge/Modality-CT-1f77b4) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2512.08029) [![Code](https://img.shields.io/badge/Code-black)](https://dingtianxingjian.github.io/clarity-project-page/?utm_source=catalyzex.com)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Tianxingjian Ding; Yuanhao Zou; Chen Chen; Mubarak Shah; Yu Tian  
  **Resumen:** Pronostica trayectorias oncológicas condicionadas al tratamiento en un espacio latente estructurado y vincula las trayectorias simuladas con recomendaciones de tratamiento conscientes del contexto.

- **[The UVA/PADOVA Type 1 Diabetes Simulator: New Features](#)**  
  ![Physio](https://img.shields.io/badge/Modality-Physio-yellow) ![Digital Twin](https://img.shields.io/badge/Modality-Digital%20Twin-lightgrey) [![Paper](https://img.shields.io/badge/Paper-blue)](#)  
  **Sede/Tiempo:** Journal of Diabetes Science and Technology, 2014  
  **Autores:** Chiara Dalla Man; Francesco Micheletto; Dayu Lv; Marc Breton; Boris Kovatchev; Claudio Cobelli  
  **Resumen:** Proporciona un simulador mecanístico de diabetes para las dinámicas de glucosa-insulina y pruebas de respuesta al tratamiento, representando un linaje importante de simulación fisiológica.

- **[EHRWorld: A Patient-Centric Medical World Model for Long-Horizon Clinical Trajectories](http://arxiv.org/abs/2602.03569)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](http://arxiv.org/abs/2602.03569)  
  **Sede/Tiempo:** arXiv, 2026  
  **Autores:** Linjie Mu; Zhongzhen Huang; Yannian Gu; Shengqian Qin; Shaoting Zhang; Xiaofan Zhang  
  **Resumen:** Entrena un modelo de mundo de EHR centrado en el paciente bajo un paradigma secuencial causal para mantener la consistencia del estado del paciente durante la simulación clínica de largo horizonte.

- **[The Patient is not a Moving Document: A World Model Training Paradigm for Longitudinal EHR](https://arxiv.org/abs/2601.22128)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2601.22128) [![Code](https://img.shields.io/badge/Code-black)](https://huggingface.co/standardmodelbio/SMB-v1-1.7B-Structure)  
  **Sede/Tiempo:** arXiv, 2026  
  **Autores:** Irsyad Adam; Zekai Chen; David Laprade; Shaun Porwal; David Laub; Erik Reinertsen; Arda Pekis; Kevin Brown  
  **Resumen:** Replantea el modelado longitudinal de EHR como una simulación del estado del paciente en lugar de una continuación de documentos, utilizando el entrenamiento de modelos de mundo para preservar las dinámicas temporales del paciente.

- **[A Clinical Environment Simulator for Dynamic AI Evaluation](#)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) ![Multimodal](https://img.shields.io/badge/Modality-Multimodal-9cf) [![Paper](https://img.shields.io/badge/Paper-blue)](#)  
  **Sede/Tiempo:** Nature Medicine, 2026  
  **Autores:** Luyang Luo; Sung Eun Kim; Xiaoman Zhang; Julius M. Kernbach; Roshan Kenia; Julian N. Acosta; Larry A. Nathanson; Adrian D. Haimovich; Adam Rodman; Ethan Goh; et al.  
  **Resumen:** Construye un simulador de entorno clínico para la evaluación dinámica de IA, proporcionando infraestructura para probar si los agentes clínicos pueden actuar de forma segura a través de escenarios evolutivos de pacientes.

- **[Beyond Generative AI: World Models for Clinical Prediction, Counterfactuals, and Planning](https://arxiv.org/abs/2511.16333)**  
  ![EHR](https://img.shields.io/badge/Modality-EHR-green) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2511.16333)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Muhammad A. Qazi; Muhammad Nadeem; Muhammad Yaqub  
  **Resumen:** Posiciona los modelos de mundo clínicos como una ruta desde la predicción generativa hacia el razonamiento contrafactual, la planificación y el soporte a la decisión clínica consciente de las intervenciones.

- **[Towards building a World Model to simulate perturbation-induced cellular dynamics by AlphaCell](https://doi.org/10.64898/2026.03.02.709176)**  
  ![Omics](https://img.shields.io/badge/Modality-Omics-brightgreen) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://doi.org/10.64898/2026.03.02.709176)  
  **Sede/Tiempo:** bioRxiv, 2026  
  **Autores:** Guohui Chuai; Xiaohan Chen; Xingbo Yang; Cheng Zhang; Kairu Qu; Wannian Li; Jingya Yang; Duanmiao Si; Feiyang Xing; Yicheng Gao; Shaliu Fu; Bing He; Qi Liu  
  **Resumen:** Introduce AlphaCell, un modelo de mundo de célula virtual que combina la representación a nivel de genoma y transiciones de estado continuo para simular respuestas a perturbaciones.

- **[Lingshu-Cell: A Generative Cellular World Model for Transcriptome Modeling toward Virtual Cells](https://arxiv.org/abs/2603.25240)**  
  ![Omics](https://img.shields.io/badge/Modality-Omics-brightgreen) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2603.25240)  
  **Sede/Tiempo:** arXiv, 2026  
  **Autores:** H. Zhang; G. H. Yuan; C. Yuan; T. Xu; T. Bian; H. Cheng; W. Huang; D. Zhao; Y. Rong  
  **Resumen:** Utiliza la difusión discreta enmascarada para modelar distribuciones de estado transcriptómico y simular respuestas de estado celular condicionadas a perturbaciones hacia el modelado de células virtuales.

- **[Artificial Intelligence Virtual Organoids (AIVOs)](#)**  
  ![Omics](https://img.shields.io/badge/Modality-Omics-brightgreen) ![Digital Twin](https://img.shields.io/badge/Modality-Digital%20Twin-lightgrey) [![Paper](https://img.shields.io/badge/Paper-blue)](#)  
  **Sede/Tiempo:** Bioactive Materials, 2026  
  **Autores:** Long Bai; Jiacan Su  
  **Resumen:** Plantea los organoides virtuales como gemelos digitales a escala de organoide que combinan células virtuales, lecturas longitudinales multimodales y módulos mecanísticos híbridos para la simulación de perturbaciones y respuesta a fármacos.

- **[GeneJepa: A Predictive World Model of the Transcriptome](https://doi.org/10.1101/2025.10.14.682378)**  
  ![Omics](https://img.shields.io/badge/Modality-Omics-brightgreen) ![World Model](https://img.shields.io/badge/World%20Model-red) ![JEPA](https://img.shields.io/badge/JEPA-purple) [![Paper](https://img.shields.io/badge/Paper-blue)](https://doi.org/10.1101/2025.10.14.682378) [![Code](https://img.shields.io/badge/Code-black)](https://github.com/BiostateAI/GeneJEPA)  
  **Sede/Tiempo:** bioRxiv, 2025  
  **Autores:** Elon Litman; Tyler Myers; Vinayak Agarwal; Ekansh Mittal; Orion Li; Ashwin Gopinath; Timothy Kassis  
  **Resumen:** Aprende un modelo de mundo predictivo estilo JEPA de transcriptomas de célula única prediciendo representaciones latentes de conjuntos de genes enmascarados para tareas relacionadas con perturbaciones.

- **[Learning Action-Conditioned World Models for Cataract Surgery from Unlabeled Videos](https://openreview.net/forum?id=aYQYOVm2AB)**  
  ![Surgical Video](https://img.shields.io/badge/Modality-Surgical%20Video-orange) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://openreview.net/forum?id=aYQYOVm2AB)  
  **Sede/Tiempo:** Medical Imaging with Deep Learning (MIDL), 2026  
  **Autores:** Nisarg A. Shah; Mingze Xia; Shameema Sikder; S. Swaroop Vedula; Vishal M. Patel  
  **Resumen:** Aprende dinámicas de video quirúrgico condicionadas a la acción en el espacio de características a partir de videos de cataratas no etiquetados utilizando tokens de acción latentes y representaciones visuales congeladas.

- **[How Far Are Surgeons from Surgical World Models? A Pilot Study on Zero-Shot Surgical Video Generation with Expert Assessment](https://arxiv.org/abs/2511.01775)**  
  ![Surgical Video](https://img.shields.io/badge/Modality-Surgical%20Video-orange) ![World Model](https://img.shields.io/badge/World%20Model-red) [![Paper](https://img.shields.io/badge/Paper-blue)](https://arxiv.org/abs/2511.01775)  
  **Sede/Tiempo:** arXiv, 2025  
  **Autores:** Ziyi Chen; Qian Xu; Jiahao Wu; Beiyang Yang; Yuhang Zhai; Guoqing Guo; Jialin Zhang; Yuxin Ding; Nassir Navab; Jiebo Luo  
  **Resumen:** Evalúa la generación de video quirúrgico zero-shot con evaluación de expertos, resaltando la brecha entre los futuros quirúrgicos visualmente plausibles y los modelos de mundo quirúrgicos clínicamente confiables.

- **[From pre-treatment to post-operative care: Leveraging digital twins for precision surgery transformation](https://linkinghub.elsevier.com/retrieve/pii/S2352648325000819)**  
  ![Digital Twin](https://img.shields.io/badge/Modality-Digital%20Twin-lightgrey) [![Paper](https://img.shields.io/badge/Paper-blue)](https://linkinghub.elsevier.com/retrieve/pii/S2352648325000819)  
  **Sede/Tiempo:** Smart Health, 2026  
  **Autores:** Farnaz Dehghan; Seyed Mojtaba Hosseini Bamakan; Mahboubeh Mirzabagheri; Alireza Naser Sadrabadi  
  **Resumen:** Describe un marco de gemelo digital que abarca la planificación preoperatoria, la guía intraoperatoria y el seguimiento postoperatorio para la cirugía de precisión.

- **[Medical Digital Twins: Enabling Precision Medicine and Medical Artificial Intelligence](#)**  
  ![Digital Twin](https://img.shields.io/badge/Modality-Digital%20Twin-lightgrey) [![Paper](https://img.shields.io/badge/Paper-blue)](#)  
  **Sede/Tiempo:** The Lancet Digital Health, 2025  
  **Autores:** C. Sadee; S. Testa; T. Barba; K. Hartmann; M. Schuessler; A. Thieme; G. M. Church; I. Okoye; T. Hernandez-Boussard; L. Hood; et al.  
  **Resumen:** Analiza cómo los gemelos digitales médicos pueden conectar la simulación individualizada, la medicina de precisión y la IA médica, destacando los desafíos traslacionales y de gobernanza.

- **[Digital Twins in Medicine](#)**  
  ![Digital Twin](https://img.shields.io/badge/Modality-Digital%20Twin-lightgrey) [![Paper](https://img.shields.io/badge/Paper-blue)](#)  
  **Sede/Tiempo:** Nature Computational Science, 2024  
  **Autores:** Reinhard Laubenbacher; Behnam Mehrad; Ilya Shmulevich; Natalia Trayanova  
  **Resumen:** Revisa los gemelos digitales médicos como simuladores individualizados, aclarando que son un vecino mecanístico y traslacional de los modelos de mundo médicos aprendidos.

- **[Digital twins for predictive oncology will be a paradigm shift for precision cancer care](https://www.nature.com/Larticles/s41591-021-01558-5)**  
  ![Digital Twin](https://img.shields.io/badge/Modality-Digital%20Twin-lightgrey) [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.nature.com/Larticles/s41591-021-01558-5)  
  **Sede/Tiempo:** Nature Medicine, 2021  
  **Autores:** Tina Hernandez-Boussard; Paul Macklin; Emily J. Greenspan; Amy L. Gryshuk; Eric Stahlberg; Tanveer Syeda-Mahmood; Ilya Shmulevich  
  **Resumen:** Sostiene que los gemelos digitales oncológicos pueden integrar datos específicos del paciente y simulaciones para pronosticar la respuesta al tratamiento y apoyar la atención oncológica de precisión.

- **[In silico clinical trials: concepts and early adoptions](https://academic.oup.com/bib/article/20/5/1699/5032454)**  
  ![Digital Twin](https://img.shields.io/badge/Modality-Digital%20Twin-lightgrey) [![Paper](https://img.shields.io/badge/Paper-blue)](https://academic.oup.com/bib/article/20/5/1699/5032454)  
  **Sede/Tiempo:** Briefings in Bioinformatics, 2019  
  **Autores:** Francesco Pappalardo; Giovanni Russo; Francesco M. Tshinanu; Marco Viceconti  
  **Resumen:** Introduce los ensayos clínicos in silico como un paradigma de simulación traslacional que conecta modelos mecanísticos, cohortes virtuales y la generación de evidencia para entes regulatorios.

- **[The Virtual Physiological Human: Ten Years After](https://www.annualreviews.org/doi/10.1146/annurev-bioeng-110915-114742)**  
  ![Digital Twin](https://img.shields.io/badge/Modality-Digital%20Twin-lightgrey) [![Paper](https://img.shields.io/badge/Paper-blue)](https://www.annualreviews.org/doi/10.1146/annurev-bioeng-110915-114742)  
  **Sede/Tiempo:** Annual Review of Biomedical Engineering, 2016  
  **Autores:** Marco Viceconti; Peter Hunter; Rod Hose  
  **Resumen:** Revisa el programa del humano fisiológico virtual y su papel en la construcción de marcos de simulación mecanísticos multiescala para el modelado biomédico individualizado.
