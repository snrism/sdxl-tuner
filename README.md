# SDXL Fine-tuning with Stability AI and Replicate

Stability AI open-sourced **SDXL**, allowing you to fine-tune diffusion models to learn patterns in input images. This Colab notebook provides a step-by-step guide to fine-tune a model using **Replicate**, either from the web or via the API.

## Requirements

Make sure you have the following installed in your environment:
```bash
!pip install replicate
```

## Set Up Replicate
Authenticate by setting your API token as an environment variable.

## Prepare Your Training Images
1. Images can be of yourself or in a particular style (e.g., illustrations).
2. Image format: JPEG or PNG.
3. Dimensions and file names don't matter.
4. Zip your images:

## Create a Model
To create a model, reuse the owner name as shown below. Set your desired model name and reuse the default visibility and hardware values. Alternatively, you can create a model directly at Replicate Create Model.

## Retrieve the Model Version
Get the model object and retrieve the latest version:

## Start the Training
Use the model version retrieved to start the training process.

## Monitor Training Progress
To follow the progress of the training job, use the following code to track the training status:

## Run the Model
Once the model has successfully trained, you can run it using the Replicate GUI or via the API:


Congratulations! Now that you have fine-tuned your own model, you can use [Replicate's SDK](https://replicate.com/docs/reference/client-libraries) or [HTTP APIs](https://replicate.com/docs/reference/http) to talk to your model from your applicaiton.
