## How to install Tensorflow on [Fedora GNU/Linux](https://getfedora.org/)
## Tensorflow instalation using [Docker](https://www.docker.com/)
 *If you don' t have docker installed, you can do this simply by ```sudo dnf install docker```*
* Download the tensorflow image: ```docker pull tensorflow/tensorflow```
* Run tensorflow: ```docker run -it -p 8888:8888 tensorflow/tensorflow```

## Tensorflow instlation via [pip](https://pypi.org/project/pip/)
* For Tensorflow with GPU Acceleration via [NVIDIA CUDA](https://en.wikipedia.org/wiki/CUDA) run: ```pip install tensorflow-gpu```
* For CPU-Only Tensorflow run: ```pip install tensorflow```

