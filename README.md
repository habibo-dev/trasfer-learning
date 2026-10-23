# TransferLab — Interactive Deep Learning Studio

TransferLab is a browser-based educational prototype for explaining CNN layers and transfer learning. It is intended for classroom demonstrations and independent study.

## What is included

- Responsive single-page interface.
- CNN convolution calculator for output shape and trainable parameter count.
- Presenter-controlled transfer-learning animation with guided lesson and free-exploration modes.
- Five manually selectable lesson stages, play/pause/restart, speed control, and a layer inspector.
- Cinematic depth styling with animated feature-flow particles.
- Transfer-learning strategy explorer: feature extraction, fine-tuning, and training from scratch.
- Qualitative controls for target-data size, source–target domain gap, and compute budget.
- Knowledge-check quiz with explanations.
- English-first academic terminology plus a short Arabic concept summary.
- Clear separation between illustrative guidance and measured results.

## Run locally

No build step is required for this first prototype:

1. Download or clone this repository.
2. Open `index.html` in a modern browser.

The page uses Google Fonts when an internet connection is available. The core interface and calculations use vanilla HTML, CSS, and JavaScript.

## Deploy

The repository can be deployed as a static site with GitHub Pages or Vercel. For GitHub Pages, choose the `main` branch and the root folder in the repository's Pages settings.

## Presenter controls

Open the **Transfer Learning** animation section. Use **Guided lesson** for a structured sequence or **Free explore** to move directly between stages. Use the timeline and Previous/Next buttons to navigate, change animation speed, and select early layers, deep layers, or the classifier head to read an explanation.

## Important scientific scope

This prototype does **not** train a neural network, load a real dataset, or report measured accuracy. Diagrams are conceptual; the CNN calculator performs mathematical calculations from the user's selected settings. Transfer-learning recommendations are qualitative hypotheses, not experimental findings.

For a research comparison, document the dataset and split policy, model architecture and pre-trained weights, preprocessing, trainable layers, optimizer, learning rate, epochs, random seeds, validation method, test metrics, class imbalance, and limitations. Evaluate competing strategies on the same held-out target test set.

## Roadmap

- Add documented dataset examples and a reproducible training notebook.
- Add an actual image-classification demo after selecting a dataset and inference approach.
- Add experiment logging and measured comparisons only after training has been run.
- Expand the lesson library with references and more interactive diagrams.


## Domain Shift Lab

The interactive Domain Shift section uses an illustrative feature-space diagram to explain how source and target representations may differ. Select a target scenario (lighting/sensor shift, plant-disease textures, satellite imagery, or an unrelated domain), adjust the illustrative gap, and toggle source/target feature clouds. The diagram is conceptual only: its positions and gap control are not empirical measurements, and it does not produce model accuracy or train a neural network.
