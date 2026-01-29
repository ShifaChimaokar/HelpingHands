<h1 align="center">Hand Movements Prediction System</h1>
<p align="center">B.E. Final Year Project(2022)</p>

For our final year major project we built a machine learning application to perform analysis of EEG(electroencephalography) signals to predict hand movements.
EEG signals record brain activity from the scalp using an EEG cap with minimal invasiveness.
Analysing these signals with respect to motor functions will allow us to predict motor functions just from the eeg recording.

## IMPLEMENTATION:
Our System can be divided into the following sub-systems:

### **Module 1 : Front-end Development Module**

The front-end of our project was developed using HTML, CSS, JavaScript and Bootstrap.This module was used to build the front-end of the project which is the GUI of our website where the user can visit and interact with our project.

### **Module 2 : Denoising and Feature Extraction Module**

The denoising and feature extraction module are responsible for data preprocessing and extracting features from that data.

There are two options for denoising signals : _The Fourier Transform_ or _The Wavelet Transform_. The Fourier Transform works well for stationary signals, but since EEG signals are changing with time and on performing various tasks, we want to use the wavelet transform as it will give us information about the signals localised in time as well as frequency domain.

The Wavelet Transform works by taking a wavelet and performing several scaling and shifting operations on our signal with it. This results in the signal being separated into low pass and high pass sub-bands. We can use this to denoise the EEG data by passing it through these filters.

Similarly it can also be used to extract features from the signal by recursively decomposing it till we obtain the required frequencies (features).


### **Module 3 : Model Training and Back-end Development Module**

The data along with features were then used to train decision tree classifiers on each label separately. These separate predictions were then combined to give the final prediction of our system.

The back-end was developed in Python using Django framework. It is a very efficient framework for machine learning tasks like ours and it is also completely open-sourced which provides an ease of debugging. Since the back-end was in python it was very easy ti integrate the various modules which were also built using python.

- Hosting : Heroku <a href="https://aiktchelpinghands.herokuapp.com/"> https://aiktchelpinghands.herokuapp.com/</a>


## SYSTEM ARCHITECTURE DESIGN:
<img width="885" height="410" alt="image" src="https://github.com/user-attachments/assets/72337951-57e4-4e38-9723-d3060450f846" />

##  Framework of Proposed System :

<img width="706" height="358" alt="image" src="https://github.com/user-attachments/assets/ee5312cb-8244-497e-9f06-68794b8e8937" />

## A Few Screenshots of the Project :
### **Landing Page :**
<img width="1436" height="806" alt="image" src="https://github.com/user-attachments/assets/d14a4ffe-aabb-4ef7-a182-049c31fe5120" />


### **About Section :**
<img width="1433" height="803" alt="image" src="https://github.com/user-attachments/assets/3320e6c2-3c56-452c-90bb-8997a1c4f0ad" />


### **I/O :**
- Section to upload the eeg data

<img width="1003" height="565" alt="image" src="https://github.com/user-attachments/assets/f8fe552c-799d-4e9d-8751-50496781d4a0" />

- File Dialogue for accepting only .csv files

<img width="1001" height="562" alt="image" src="https://github.com/user-attachments/assets/f64cf3cf-3123-4c5a-9337-860ccf80c69e" />

- Uploaded EEG data 

<img width="1005" height="565" alt="image" src="https://github.com/user-attachments/assets/4affec08-5c8f-4179-8b91-9b9b4b7e2ae0" />

- Sample Output 1

<img width="1002" height="564" alt="image" src="https://github.com/user-attachments/assets/e882b542-272b-425a-a86d-e8d56a68fb2f" />

- Sample Output 2

<img width="1000" height="558" alt="image" src="https://github.com/user-attachments/assets/f7dac6c2-5fdb-4072-9b48-7ede87fa062d" />

- Sample Output 3

<img width="1001" height="564" alt="image" src="https://github.com/user-attachments/assets/9ce0dc87-1406-4864-b390-7a3142f64e3a" />

- Sample Output 4

<img width="861" height="484" alt="image" src="https://github.com/user-attachments/assets/3e3df423-7b01-4df8-8abf-11793ed05592" />


## REFERENCES :

- A. W. Pise and P. P. Rege, "Comparative Analysis of Various Filtering Techniques for Denoising EEG Signals," 2021 6th International Conference for Convergence in Technology (I2CT), 2021, pp. 1-4, doi: 10.1109/I2CT51068.2021.9417984.
- R. Chatterjee and T. Bandyopadhyay, "EEG Based Motor Imagery Classification Using SVM and MLP," 2016 2nd International Conference on Computational Intelligence and Networks (CINE), 2016, pp. 84-89, doi: 10.1109/CINE.2016.22.
- A. Prochazka, J. Kukal and O. Vysata, "Wavelet Transform Use for Feature Extraction and EEG Signal Segments Classification," 2008 3rd International Symposium on Communications, Control and Signal Processing, 2008, pp. 719-722, doi: 10.1109/ISCCSP.2008.4537317.
- Dataset : <a href="https://doi.org/10.1038/sdata.2014.47">https://doi.org/10.1038/sdata.2014.47</a>
- Electroencephalography : <a href="https://en.wikipedia.org/wiki/Electroencephalography">https://en.wikipedia.org/wiki/Electroencephalography</a>
- EEG vs MRI vs fMRI : <a href ="https://imotions.com/blog/eeg-vs-mri-vs-fmri-differences/">https://imotions.com/blog/eeg-vs-mri-vs-fmri-differences/</a>


## CONTRIBUTORS:

- **Janvi Karia**<br>
[-] GitHub : <a href="https://github.com/janvi2001">https://github.com/janvi2001</a>

- **Misbah Shaikh**<br>
[-] GitHub : <a href="https://github.com/misbah46">https://github.com/misbah46</a>

- **Shifa Chimaokar**<br>
[-] GitHub : <a href="https://github.com/ShifaChimaokar">https://github.com/ShifaChimaokar</a>

- **Master Farheen**<br>
