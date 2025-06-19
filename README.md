## RUN IT IN POWER SHELL as Administrator
- If you get error by activating venv run to check status: Get-ExecutionPolicy
- Than run to solve issue: Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted -Force


## MY HARDWARE ADD TOURCH VERSION

- PyTorch Version: 2.5.1+cu121
- CUDA verfügbar: True
- CUDA Version: 12.1
- GPU: Quadro RTX 5000

## DATASET

# Download dataset
https://www.kaggle.com/datasets/subhamshome/esa-hubble-images-3-classes
# Put galaxy images inside: data\esa_hubble\galaxies
# Note: For GAN generation, I used nebula images as an alternative dataset.
#       If you want to set up the dataset for the GAN method,
#       place nebula images inside: data\esa_hubble\nebulae\all
# Optional
https://www.kaggle.com/datasets/jaimetrickz/galaxy-zoo-2-images

## INSTALLATION
# Install Python 3.10
# Create a virtual environment and activate it

pip install -r requirements.txt

# OR

python.exe -m pip install --upgrade pip
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121

pip install matplotlib

## HOW TO USE:
# Use notebooks/CNN_develop.ipynb to set up the CNN, and notebooks/GAN_develop.ipynb for the GAN.
# For simplicity, the number of epochs has been set to low values.
# CNN 200 epochs training time 289m 17.5s
# GAN 250 epochs training time 148m 10.5s
# The model weights are located in the models folder.

