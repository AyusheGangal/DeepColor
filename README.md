# DeepColor
This is the mplementation of Google's Inception ResNet v2 for the task of automatic colorization of gray-scale images. The task-at-hand is treated as a classification problem and uses CIELAB color space for assigning colors to the pixels.

The dataset consists of two compressed zip files:
1. ab.zip : This contains 25 .npy files consisting of a and b dimensions of LAB color space images, of the MIRFLICKR25k randomly sized colored image dataset. The LAB color space generally takes up large disk spaces, hence is a lot slower to load. That is the reason, I divided this into 25 files, so that it can be loaded at the time of requirement.
2. l.zip : This consists of a gray_scale.npy file which is the grayscale version of the MIRFLICKR25k dataset.

The image dataset which I used was taken from the MIRFLICKR25k.

The following steps should be followed to run the 'DeepColor' system:
1. Download the dataset from the link in the 'DeepColor/Data.txt'.
2. In order to successfully run the system locally:
    - Install Python3
    - Set the correct path for the dataset by altering the file path to be the location of the dataset in the file explorer/finder.

3. To run the the system in google colab: 
    - Import the downloaded dataset in your drive.
    - Run the cells in the iPython notebook and mount the drive by entering your credentials.
    - set the correct path to the dataset in the drive by altering the file path.

