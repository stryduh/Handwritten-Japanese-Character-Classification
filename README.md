# Handwritten Japanese Character Classification
## About the Project
Implement and train convolutional neural networks (CNN) for the classification of handwritten hiragana and katakana characters in PyTorch.
Hiragana class contains 71 character classes and katakana class contains 48 character classes. 2 CNNs are trained, one for each of hiragana and katakana.
## Technologies Used
- Python 
- PyTorch
- Numpy
- Matplotlib
- PIL
## Data and Code
The datasets are provided by the ETL japanese character database at http://etlcdb.db.aist.go.jp/.
Specifications about each dataset can also be found on the same website and are also outlined in the Data-Extraction notebooks.
ETL1_Katakana.ipynb extracts the katakana characters from the ETL datasets and saves them to katakana.npz. ETL8_Hiragana.ipynb performs a similar task for hiragana.
hiragana.npz and katakana.npz are then used to train the convolutional neural networks for their respective classification tasks. To be able to run the model code from
Pytorch_Hiragana.ipynb and Pytorch_Katakana.ipynb in Google Colab, the files hiragana.npz and katakana.npz must be uploaded to your Google Drive or can be saved locally
if you wish to run on a local runtime.
## Results
The katakana CNN classified 12714/13968 characters correctly for a test accuracy of 91.02%. The hiragana CNN classified 1847/2130 characters correctly for a test
accuracy of 86.71%. 
## Further Work
Data augmentation for the hiragana dataset may be considered as the hiragana dataset is much smaller than the katakana dataset while having more more classes.  






