# Image Classification with PyTorch

Image classification is one of the most beginner-friendly practice for deep learning. In one of my laboratories
in [PCZ](https://pcz.pl), I have been asked to develop a neural network project. I chose to do image classification by
using PyTorch and a [publicly available dataset](https://www.kaggle.com/datasets/asdasdasasdas/garbage-classification).

I mainly used neural networks with convolutional layers, the layers that will extract features. To classify, I simply
added some dense layers at the end. I didn't include every architecture I tried into this notebook, but they were more
or less similar.

Project includes different utilities like *plotting sample images*, *custom training function*, *saving* and *loading
checkpoint* options etc. These can be directly copied and used in new projects. Actually I'm thinking to develop a
richer utility package in order to not hassle with the tiny details too much later on. Validation patience was one of
the things that I was going to implement here, but then decided not to. If someone wants to contribute to project
somehow, this could be the thing you can work on.

## Run

After downloading the project, it is advised you to create a virtual environment, possibly `virtualenv`.

```bash
python3 -m venv venv && source venv/bin/activate
```

Install the requirements, and you are good to go!

```bash
pip install -r requirements
```

> Please note that, even though notebook supports GPU usage, the torch you will download from `requirements.txt` is CPU
only. Alternatively you can download torch with cuda support from the [official webpage](https://pytorch.org/).  