# Cuda simple installation guide for Debian 9 (in order to be able to work with Tensorflow)

A short reminder on how to quickly install cuda toolkit and cudnn library on Debian 9 for Tensorflow

## Step 1

Install nividia cuda toolkit from non contrib sources (add it if not done already, simplest way is through graphical interface)

```bash
sudo apt install nvidia-cuda-toolkit
```

## Step 2

Register (if not already done) and download the .deb (CuDNN v 6 for Tensorflow to work)

[cuDNN](https://developer.nvidia.com/rdp/cudnn-download)

## Step 3

Install the .deb previously dowload using gdebi

```bash
sudo gdebi #NAME_OF_FILE#
```

## Step 4

Follow installation guide from tensorflow (create virtual env before doing this command)
[Tensorflow install guide](https://www.tensorflow.org/install/install_linux#InstallingVirtualenv)

Note: inside the virtual env, you can use pip alone (and not pip3)

