# flower-species-recognition

Flower species recognition on Tensorflow.

## 🛒 Requires

- Python3
- PIP3

## 🍽 Usage

```python
python3 -m scripts.label_image \
    --graph=tf_files/models/retrained_graph.pb  \
    --image=examples/102501987_3cdb8e5394_n.jpg
```

Response should be like to;

```
Evaluation time (1-image): 0.854s

roses (score=0.99468)
tulips (score=0.00438)
sunflowers (score=0.00074)
daisy (score=0.00017)
dandelion (score=0.00003)
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