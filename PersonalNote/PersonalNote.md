Markdown: https://www.runoob.com/markdown/md-tutorial.html

This solution comes from https://www.bilibili.com/video/BV16Z4y1i7vv?p=22

Install Python and use Jupter notebooks in Window
Download Python from office website: https://www.python.org/downloads/windows/ (My laptop is for 64-bit Installer)
Type [pip install ipykernel] in the window terminal and thus you can run .ipynb in the local.

Before implement the program as the following code, need to set the envirment in VScode.

First, create a new python virtual environment and open it. Please type the following instructions in the terminal.
python -m venv cnn_venv
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
.\cnn_venv\Scripts\Activate (or use complete path)

Now that your virtual environment is activated, you need to install ipykernel to allow Jupyter to interact with your virtual environment
pip install ipykernel

Add your virtual environment to Jupyter's kernel list
python -m ipykernel install --user --name=cnn_venv

Run the following command to install Jupyter 
pip install notebook
jupyter notebook

Then restart VS Code. After it, in the top right corner, you will find a dropdown list where you can select a kernel. Make sure to select the kernel that matches your virtual environment

Open the python virtual environment again and start to install related packages
pip install numpy
pip install pandas
pip install torch torchvision torchaudio (For CPU)
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118 (For GPU) (See https://pytorch.org/get-started/locally/)
pip install matplotlib

Use the following instruction to quiz the virtual python environment
deactivate