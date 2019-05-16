# tensorflow-textgenrnn-gpu
Last updated: 2019/05/16

This repository creates a docker container with a customized tensorflow version with suport for GPU compute 3.0 and [textgenrnn](https://github.com/minimaxir/textgenrnn) to develop deep learning text analysis.

The customized tensorflow wheel is created using [this github repo](https://www.github.com/stealthizer/tensorflow_builder).

To use this docker you can run from the location of your app:
```
docker run --ti --runtime=nvidia -v $(pwd):/app stealthizer/tensorflow-textgenrnn-gpu python3 /app/your_app.py
```
