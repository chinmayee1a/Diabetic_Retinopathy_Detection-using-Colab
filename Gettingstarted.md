Steps to Execute in Google Colab
Step 1: Open the Notebook
Use this link: https://colab.research.google.com/drive/1_BvUiFZlatdaZusk_MYgBF0AdpxXw8-p

Step 2: Enable GPU and High RAM
Go to Runtime > Change runtime type

Select:

Hardware accelerator: GPU

(Optional) Choose "High-RAM" runtime

Step 3: Authenticate Google Drive
The notebook uses PyDrive to download .npy data files.

Follow prompts to authenticate your Google account when executing:

python
Copy
Edit
from pydrive.auth import GoogleAuth
...
Step 4: Run the Notebook
Click Runtime > Run all

This will:

Load the dataset

Train a CNN model

Evaluate and visualize results

Step 5: Review Results
View predicted labels on test images

Analyze training vs. validation accuracy and loss

Note the printed test accuracy (final model evaluation)
