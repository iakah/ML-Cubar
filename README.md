# Nerfstudio Gradio WebUI

## Introduction

This repository provides a user-friendly web interface for [Nerfstudio](https://github.com/nerfstudio-project/nerfstudio) using the [Gradio](https://gradio.app/) library. The Nerfstudio Gradio WebUI allows users to easily train, visualize, process data, and export models without the need for complex command-line interactions.

## Features

- **Training**: Train Nerfstudio models directly from the web interface by selecting the dataset path and corresponding data parser.
- **Visualization**: Visualize trained models with Viser.
- **Data Processing**: Process training data by selecting the dataset path, output path, and processing method.
- **Model Export**: Export trained models by selecting the model configuration and output path.

## Installation

1. Ensure that you have Nerfstudio (version >= 1.10) installed and set up properly: [https://docs.nerf.studio/](https://docs.nerf.studio/)

2. Install the required dependencies by running the following command in the Nerfstudio environment:

   ```bash
   pip install gradio
   ```
   
3. Install FFmpeg based on your operating system:
  - Ubuntu/Debian: Use package manager
  - MacOS: Use Homebrew
  - Windows: Use Chocolatey or download from official website

4. Refer to the Nerfstudio documentation for specific COLMAP installation instructions:
  [Nerfstudio Custom Dataset Guide](https://docs.nerf.studio/quickstart/custom_dataset.html)


5. Clone this repository.

## Usage

1. Start the Nerfstudio Gradio WebUI by running the following command (Add --help to see more options):

   ```bash
   python webui.py
   ```

2. Open a web browser and navigate to `http://localhost:7860` to access the WebUI.

3. Use the different tabs in the WebUI to perform various tasks:

   - **Training**: Select the dataset path and corresponding data parser, then click the "Train" button to start training. Monitor the training progress in the terminal.

   - **Visualization**: Choose the "Visualize" tab, select the configuration file for the trained model, and click the "Visualize" button to launch the Viser tool.

   - **Data Processing**: Choose the "Process Data" tab, select the dataset path, output path, and processing method. Click the "Submit" button to create a new folder if the output path doesn't exist. Then, click the "Process" button to start processing the data.

   - **Model Export**: Choose the "Export" tab, select the configuration file for the trained model and the output path. Click the "Export" button to start exporting the model.

4. Explore the different functionalities provided by the WebUI and enjoy a seamless experience with Nerfstudio!

## Platforms

Tested on Windows with 3070 and Linux with 2080ti. Multi-GPU untested. Subprocesses may not run properly on Windows when processing data.
