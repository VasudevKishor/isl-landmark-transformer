# SignLink AI (VoxISL) ── `isl-landmark-transformer`

> **Slogan:** *"Bridging Silence with Structure: Real-Time ISL to English Translation."* > **Domain:** Neural Networks & Deep Learning (NNDL) • Computer Vision (CV) • Natural Language Processing (NLP)

---

## 🧠 Project Abstract & Solution
Indian Sign Language (ISL) is a rich, structural visual-spatial language with its own native non-linear grammar, spatial morphology, and unique syntax structures. The key barrier is a systemic lack of sign-literacy within public, corporate, and educational environments.

`isl-landmark-transformer` is an end-to-end, deep learning pipeline that shifts sign translation away from traditional brute-force video classification. By processing high-fidelity hand and body coordinate markers extracted on the edge, it transforms live inputs into lightweight temporal streams. These signatures are processed via a sequence-to-sequence Deep NLP model, producing contextually accurate and grammatically sound English text and spoken audio.

---

## 🛠️ Deep Learning Architecture Pipeline

The architecture utilizes a hybrid spatial-temporal network split into three main computation segments:

```text
[Webcam Stream] ──(MediaPipe Edge)──> [3D Spatial Coordinates]
                                               │
                                      (Normalization Engine)
                                               │
                                               ▼
[Target English Sentence] <──(Transformer) <── [Bi-GRU Encodings]
