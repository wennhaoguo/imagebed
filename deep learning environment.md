# deep learning environment

## pytorch in virtual environment of conda

  在Linux上使用conda虚拟环境安装PyTorch，可以按照以下步骤进行：

1. 激活你的conda环境。使用以下命令激活你的环境，替换"your_env_name"为你创建的conda环境的名称：

   bash

```
conda activate your_env_name
```

安装PyTorch。在激活的环境下，运行以下命令安装适合你系统和硬件的PyTorch版本。你可以在PyTorch官方网站上找到正确的安装命令：<https://pytorch.org/get-started/locally/>

例如，对于CUDA 11.1(nvidia-smi to see the cuda version)的Linux系统，可以运行：

```
bash
```

```
conda install pytorch torchvision torchaudio cudatoolkit=11.1 -c pytorch
```

这将安装PyTorch、torchvision和torchaudio，同时确保与CUDA 11.1兼容。

验证安装。在安装完成后，你可以在Python交互式环境中验证PyTorch是否成功安装：

```
bash
```

```
python
```

然后在Python中执行以下代码：

```
python
```

1. `import torch print(torch._version_)`

2. 如果没有报错，并且成功打印出PyTorch的版本号，说明安装成功。

这样，你就在你的conda虚拟环境中成功安装了PyTorch。

## miniconda

<https://zhuanlan.zhihu.com/p/541309324>