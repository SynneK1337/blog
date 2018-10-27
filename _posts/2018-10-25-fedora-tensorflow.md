---
layout: post
title:  "Tensorflow installation guide for Fedora GNU/Linux"
tags:
  - Fedora
  - Linux
  - GNU/Linux
  - Tensorflow
  - AI
  - Machine Learning
  - Artifical Inteligence
  - Google Code-In
hero: uploads/tensorflowfedora.png
overlay: blue
published: true

---
<!–-break-–>
## How to install Tensorflow on [Fedora GNU/Linux](https://getfedora.org/)
* Download *virtualenv* by executing ```sudo pip3 install virtualenv```

* As first you have to get 3.6 version of python interpreter. You can do it by executing ```sudo dnf install python36.x86_64```

* Create virtualenv with older python by ```virtualenv --system-site-packages -p /usr/bin/python3.6 ./venv && source ./venv/bin/activate```

* For Tensorflow with GPU Acceleration via [NVIDIA CUDA](https://en.wikipedia.org/wiki/CUDA) run: ```pip install tensorflow-gpu``` ***You have to install another libraries shown down below!***

* For CPU-Only Tensorflow run: ```pip install tensorflow```

* To execute app designed using tensorflow just run ```python3.6 app.py```

* To go out of virtualenv run ```deactivate```

## Installing libraries for CUDA Acceleration inside *tensorflow*

* Install GPU Drivers like in this [article](https://fedoramagazine.org/install-nvidia-gpu/)

* Install CUDA Toolkit by ```wget https://developer.nvidia.com/compute/cuda/10.0/Prod/local_installers/cuda_10.0.130_410.48_linux && sudo sh cuda_10.0.130_410.48_linux```

* Install cuDNN **(You must be inside NVIDIA Developer Program)**:
    * [Register](https://developer.nvidia.com/cudnn) into Developer Program and download cuDNN into seperate folder
    * ```cd <folder where you downloaded it>```
    * ```tar -xzvf cudnn-9.0-linux-x64-v7.tgz```
    * ```sudo cp cuda/include/cudnn.h /usr/local/cuda/include```
      ```sudo cp cuda/lib64/libcudnn* /usr/local/cuda/lib64```
      ```sudo chmod a+r /usr/local/cuda/include/cudnn.h /usr/local/cuda/lib64/libcudnn*```
## Test the installation
* Create test.py
  ```
      import tensorflow as tf


      class SquareTest(tf.test.TestCase):

        def testSquare(self):
          with self.test_session():
            x = tf.square([2, 3])
            self.assertAllEqual(x.eval(), [4, 9])


      if __name__ == '__main__':
        tf.test.main()
  ```

* ```python3.6 test.py```