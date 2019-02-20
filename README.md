# 💐 flower-species-recognition

Flower species recognition on Tensorflow.

#### You can training an another image recognition model on this source.

## ⚡ Installation

Via [GIT](https://git-scm.com/)

```bash
$ git clone https://github.com/voyula/flower-species-recognition.git
$ cd flower-species-recognition
```

## 🛒 Requires

- Python3
- PIP3

## 🍽 Usage

```bash
python3 -m scripts.label_image \
    --graph=tf_files/models/retrained_graph.pb  \
    --image=examples/102501987_3cdb8e5394_n.jpg
```

Should be response like to;

```
Evaluation time (1-image): 0.854s

roses (score=0.99468)
tulips (score=0.00438)
sunflowers (score=0.00074)
daisy (score=0.00017)
dandelion (score=0.00003)
```
## 🎯 Training of the new model (Optional)

```bash
python3 -m scripts.retrain \
  --bottleneck_dir=tf_files/bottlenecks \
  --how_many_training_steps=500 \
  --model_dir=tf_files/models/ \
  --summaries_dir=tf_files/training_summaries/"${ARCHITECTURE}" \
  --output_graph=tf_files/retrained_graph.pb \
  --output_labels=tf_files/retrained_labels.txt \
  --architecture="${ARCHITECTURE}" \
  --image_dir=tf_files/flower_photos
```

### 📜 Standards

- [Semantic Versioning 2.0.0](https://semver.org/)

### 🛠 Contributing

See [CONTRIBUTING](CONTRIBUTING.md) file for details.

### 🎙 Credits

- [voyula](https://github.com/voyula)
- [All Contributors](../../contributors)

### 📌 License

Licensed under the MIT License. See [License File](LICENSE.md) for more information.

Based on [tensorflow-for-poets](https://codelabs.developers.google.com/codelabs/tensorflow-for-poets)
