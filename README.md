# NVIDIA AI Workbench: Introduction
This is an [NVIDIA AI Workbench](https://developer.nvidia.com/blog/develop-and-deploy-scalable-generative-ai-models-seamlessly-with-nvidia-ai-workbench/) example Project that demonstrates how to train a Large Language Model to annotate large sections of text with realistic punctuation and capitalization using the NeMo Framework. We will conduct data preprocessing, model configuration, model training, and model inference on new text to evaluate performance. Users in the [AI Workbench Early Access Program](https://www.nvidia.com/en-us/deep-learning-ai/solutions/data-science/workbench/) can get up and running with this Project in minutes.

System Requirements:
* Operating System: Ubuntu 22.04
* CPU requirements: None, tested with Intel&reg; Xeon&reg; Gold 6240R CPU @ 2.40GHz
* GPU requirements: Any NVIDIA training GPU, tested with NVIDIA A100-40GB
* NVIDIA driver requirements: Latest driver version
* Storage requirements: 40GB

If you have NVIDIA AI Workbench already installed, you can use this Project in AI Workbench on your choice of machine by:
1. Forking this Project to your own GitHub namespace and copying the link

   ```https://github.com/[your_namespace]/<project_name>```
   
3. Opening a shell and activating the Context you want to clone into by

   ```$ nvwb activate <desired_context>```
   
5. Cloning this Project onto your desired machine by running

   ```$ nvwb clone project <your_project>```
   
7. Opening the Project by

   ```$ nvwb open <project_name>```
   
9. Starting JupyterLab by

   ```$ nvwb start jupyterlab```

The notebook(s) in this project were adapted from the NVIDIA NeMo Github repository, which can be found [here](https://github.com/NVIDIA/NeMo/tree/main/tutorials/nlp).

## NeMo Frameworks: Punctuation and Capitalization
Automatic Speech Recognition (ASR) systems typically generate text with no punctuation and capitalization of the words. This tutorial explains how to implement a model in NeMo that will predict punctuation and capitalization for each word in a sentence to make ASR output more readable and to boost performance of the named entity recognition, machine translation or text-to-speech models. We'll show how to train a model for this task using a pre-trained BERT model. For every word in our training dataset we’re going to predict:

* punctuation mark that should follow the word and

* whether the word should be capitalized

## Getting Started
Navigate to the code directory of the project. Then, open the notebook titled ```Punctuation_and_Capitalization.ipynb``` and get started. Happy coding!

**Note:** This notebook has been tested with an NVIDIA A100-40gb GPU and the following version of NVIDIA AI Workbench: ```nvwb 0.2.66 (internal; linux; amd64; go1.18.10; Tue Sep 12 18:50:21 UTC 2023)```

## License
This NVIDIA AI Workbench example project is under the [Apache 2.0 License](https://github.com/nv-edwli/nemo-punctuation/blob/main/LICENSE.txt)
