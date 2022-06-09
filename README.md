# dino_bone_finding_OpenVINO

## Notebook Contents

This notebook demonstrates how to convert a Pytorch model for dinasour bone finding based on a Google Map, to ONNX then to IR files to run inference with OpenVINO.

The dinasour bone finding map is trained with Resnet18 against data collected from central New Mexico. The waypoint information is NOT provided. The real challenge is to SCORE similar geological depositional envirnoments in other parts of the US - for example in Utah.

In this notebook, the trained Pytorch model is first converted to ONNX format and then to IR files with FP16. Inference results are then compared using Pytorch, ONNX and IR formats on a single Image for classifying the image with a confidence score. Performance on 20 images are further compared between the 3 formats, to demonstrate the inference speeding with OpenVINO. Finally, inferencing performance is compared with the 3 formats on a 224 map folder, and the final results could be merged into a large map to observe the results for indicating the possbile spots to find dinasour bones.



## Installation Instructions

If you have not done so already, please follow the [Installation Guide](../../README.md) to install all required dependencies.
