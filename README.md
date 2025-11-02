# aiprojects
Personal AI Projects


SadTalker Google Colab Quick Demo
This notebook provides a quick demonstration of how to use SadTalker, a method for generating realistic and stylized talking head videos from a single image and audio.

Based on the original GitHub repository: https://github.com/Winfredy/SadTalker

Installation
The installation process involves several steps to set up the environment and download the necessary models.

Check CUDA Availability: The notebook first verifies that a GPU is available and configured in the notebook settings.
Install Dependencies: This step installs various Python packages and system dependencies using pip and apt-get. This includes:
Setting up Python 3.8.
Installing python3.8-distutils.
Upgrading setuptools and wheel.
Installing core requirements from requirements.txt, including numpy, face_alignment, imageio, librosa, numba, resampy, pydub, scipy, kornia, tqdm, yacs, pyyaml, joblib, scikit-image, basicsr, facexlib, gradio, gfpgan, av, and safetensors.
Installing filterpy.
Installing basicsr, facexlib, and gfpgan.
Download Pre-trained Models: This step downloads the pre-trained models required for SadTalker to function correctly, including mapping_00109-model.pth.tar, mapping_00229-model.pth.tar, SadTalker_V0.0.2_256.safetensors, and SadTalker_V0.0.2_512.safetensors, as well as models for GFPGAN.
Usage
Choose Source Image: You can select a source image from the provided examples in the examples/source_image directory using an interactive dropdown widget.
Run Animation: The inference.py script is executed with the chosen source image and a driven audio file (./examples/driven_audio/RD_Radio31_000.wav in this demo) to generate the talking head video. The output video is saved in the ./results directory.
Visualize Result: The generated video animation is displayed within the notebook.
Note
The installation process may take some time depending on your internet connection and the Colab environment.
