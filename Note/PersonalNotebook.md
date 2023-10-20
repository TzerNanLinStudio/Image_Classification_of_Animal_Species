# 1. Markdown Instruction Manual

Online Resource 1 : https://www.runoob.com/markdown/md-tutorial.html

# 2. Machine Learning Study Resource

Online Resource 1 : https://www.bilibili.com/video/BV16Z4y1i7vv?p=22

Online Resource 2 : https://www.youtube.com/playlist?list=PLJV_el3uVTsMhtt7_Y6sgTHGHp1Vb2P2J


# 3. Machine Learning Environment Setup

# 3.1. Downloading Python

Begin by downloading Python from the official website: Python Downloads for Windows. Ensure you select the 64-bit installer if your laptop supports it.

# 3.2. Installing ipykernel

Launch the Windows terminal and type the following command in the terminal. It will allow you to execute .ipynb files locally.

```
pip install ipykernel
```

# 3.3. Setting Up the environment in VSCode

# 3.3.1. Creating a virtual environment

To create a new Python virtual environment and activate it, enter the following commands in the terminal.

```
python -m venv cnn_venv
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
.\cnn_venv\Scripts\Activate 
```

# 3.3.2. Installing ipykernel 

With the virtual environment activated, install ipykernel to enable Jupyter to interact with it.

```
pip install ipykernel
```

# 3.3.3. Integrating with Jupyter
In the virtual environment, add your virtual environment to Jupyter's list of kernels.

```
python -m ipykernel install --user --name=cnn_venv
```

# 3.3.4. Installing and Launching Jupyter

In the virtual environment, use the following commands to install and launch Jupyter.

```
pip install notebook
jupyter notebook
```

# 3.3.5. Exiting the virtual environment

In the virtual environment, after following and executing the previous commands, using the following command to exit the virtual environment.

```
deactivate
```

# 3.3.6. VSCode Configuration

After completing the previous steps, restart VS Code. In the top right corner, there will be a dropdown list for kernel selection. Please pick the kernel corresponding to the virtual environment.

# 3.4. Package Installation

# 3.4.1. Reactivate your virtual environment

Once back in VSCode, reactivate the virtual environment to begin the installation of necessary packages.

```
.\cnn_venv\Scripts\Activate 
```

# 3.4.2. Installing Dependencies

In the virtual environment, use the following commands to install the necessary packages. Refer to: https://pytorch.org/get-started/locally/ for detailed installation of PyTorch.

```
pip install numpy
pip install pandas
pip install torch torchvision torchaudio # For CPU version
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118 # For GPU version 
pip install matplotlib

```
