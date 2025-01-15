# Learning Section:
Welcome to the learning section, this is a breakdown of each example in this directory.

## Librosa Example Explained:

Librosa is a library built in Python that allows a user to load an audio file and show the waveforms that exist. Before we run anything, please ensure that the packages below have been installed and run onto your Jupyte Notebook Kernel:

![image](https://github.com/user-attachments/assets/172e4cd1-663d-4486-bab3-427d9dab50cb)


When loaded, the default graph that is shown is an Amplitude vs. Time graph. (as shown below)

![image](https://github.com/user-attachments/assets/f61d61d9-543d-48d5-9566-85dcfa183552)

**Note**: The .wav file that I used in this was a song that I had on my local computer. You can pretty much use any music file you want. 

### A couple of things to explain:
1.) When you first load a wav file into librosa using the "load" function, a signal and sample rate (sr) is returned. 
  - **Signal**: A 1-Dimensional array that is spans a size of Sample Rate * Time
  - **Sample Rate**: The number of samples taken from the inputted audio file (default: 22050)

2.) librosa.display.waveshow will take in the signal and allow for a visualization of the audio data. [More Info](https://librosa.org/doc/main/generated/librosa.display.waveshow.html)

3.) matplotlib (aka plt) allows for the customization of the axes as well as the ultimate showing of the waveform

