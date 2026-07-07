# AI Teaching Widgets

Interactive HTML widgets created by AI for teaching Machine Learning, Artificial Intelligence, and other technology areas. Each widget is a self-contained demo — no installation required. Click any link below to open it directly in your browser.

Hosted on GitHub Pages: **https://mtgca.github.io/widgets_pubic/**

---

## Table of Contents

| Widget | Topic | Status | Description |
|--------|-------|--------|-------------|
| [LLM Next-Word Prediction](https://mtgca.github.io/widgets_pubic/llmpretraining.html) | AI / LLMs | ✅ Verified | Visualizes LLM pretraining via next-token prediction over text corpus. |
| [External Clustering Metrics: ARI & NMI](https://mtgca.github.io/widgets_pubic/external_metrics_interactive.html) | ML / Clustering | ✅ Verified | Drag-and-drop demo of Adjusted Rand Index and Normalized Mutual Information on cluster assignments. |
| [GMM Covariance Types](https://mtgca.github.io/widgets_pubic/gmm_covariance_interactive.html) | ML / Clustering | ✅ Verified | How covariance matrix types (full, tied, diagonal, spherical) shape GMM clusters. |
| [EM Algorithm for GMMs](https://mtgca.github.io/widgets_pubic/gmm_em_interactive.html) | ML / Clustering | ✅ Verified | Step-through visualization of EM fitting a Gaussian Mixture Model to data. |
| [Hierarchical Clustering Linkage Methods](https://mtgca.github.io/widgets_pubic/linkage_methods_interactive.html) | ML / Clustering | ✅ Verified | Compares single, complete, average, and Ward linkage for hierarchical dendrograms. |
| [Learning Rate Scheduling](https://mtgca.github.io/widgets_pubic/Learning_Rate_Scheduling.html) | AI / Deep Learning | ✅ Verified | Compare learning rate decay strategies: cosine annealing, SGDR, step, exponential, warm-up. |
| [Dropout Regularization](https://mtgca.github.io/widgets_pubic/dropout.html) | AI / Deep Learning | ✅ Verified | How dropout randomly deactivates neurons during training to prevent overfitting. |
| [Convolution Visualizer](https://mtgca.github.io/widgets_pubic/conv.html) | AI / Deep Learning | ✅ Verified | Kernel sliding over input matrix to produce feature map in 2D convolution. |
| [CNN Output Size Calculator](https://mtgca.github.io/widgets_pubic/cnn_output_calculator.html) | AI / Deep Learning | ✅ Verified | Compute CNN layer output dimensions given kernel size, padding, and stride. |
| [Intuitive CNN Feature Map](https://mtgca.github.io/widgets_pubic/cnn_intuition.html) | AI / Deep Learning | ✅ Verified | 3D visualization of convolution kernel scanning input grid to build feature map. |
| [Normalization Techniques](https://mtgca.github.io/widgets_pubic/normalization_techniques.html) | AI / Deep Learning | ✅ Verified | Compare Batch, Layer, Instance, and Group Normalization on (N, C, H, W) tensors. |
| [CNN Building Blocks](https://mtgca.github.io/widgets_pubic/cnn_architecture_blocks_interactive.html) | AI / Deep Learning | ⚠️ AI-only | Evolution of CNN building blocks from LeNet to ConvNeXt with timeline and comparison. |
| [Types of Sequential Models](https://mtgca.github.io/widgets_pubic/sequential_models_interactive.html) | AI / Deep Learning | ✅ Verified | Compare many-to-one, one-to-many, and many-to-many sequence models with examples. |
| [RNNs: Unrolling the Computational Graph](https://mtgca.github.io/widgets_pubic/rnn_unrolling_interactive.html) | AI / Deep Learning | ✅ Verified | Unroll recurrent cell feedback loop over time with native MathML and parameter sharing. |
| [RNNs: Hidden-State & Output Update — Matrix Shapes](https://mtgca.github.io/widgets_pubic/rnn_matrix_shapes_interactive.html) | AI / Deep Learning | ✅ Verified | Interactive explorer of RNN update equations: choose dimensions, see weight matrices and dot products. |
| [RNNs: Character-Level Language Modeling](https://mtgca.github.io/widgets_pubic/rnn_char_lm_interactive.html) | AI / Deep Learning | ✅ Verified | Train tiny RNN on "hello": step through training, inference, and temperature playground. |
| [BPTT: Vanishing & Exploding Gradients](https://mtgca.github.io/widgets_pubic/bptt_gradients_interactive.html) | AI / Deep Learning | ⚠️ AI-only | Slide eigenvalue and sequence length to watch gradients amplify or vanish through time. |
| [From Vocabulary to Embedding: Embedding vs Linear Layers](https://mtgca.github.io/widgets_pubic/vocab_to_embedding_interactive.html) | AI / Deep Learning | ✅ Verified | Token journey from vocabulary to embedding; compare lookup and linear layer costs. |
| [Semantic Vector Spaces: The Geometry of Meaning](https://mtgca.github.io/widgets_pubic/semantic_vector_spaces_interactive.html) | AI / Deep Learning | ✅ Verified | Word embedding semantics: heatmap, 2D projections, nearest neighbors, and king − man + woman. |
| [How Word Embeddings Are Learned: Train a Tiny Next-Word Predictor](https://mtgca.github.io/widgets_pubic/embedding_training_interactive.html) | AI / Deep Learning | ✅ Verified | Train embedding model in browser; watch 8D space self-organize, explore weight tying and gotchas. |

**Status legend:** ✅ **Verified** — reviewed for correctness by a human expert in the field. ⚠️ **AI-only** — generated by AI and *not yet* verified by an expert; use with a critical eye.

---

## About

All widgets are single-file HTML apps with embedded CSS and JavaScript — no frameworks, no build step. They are designed to be used in class as interactive lecture aids or assigned as self-study explorations.

Contributions welcome. See [CLAUDE.md](CLAUDE.md) for conventions on adding new widgets.
