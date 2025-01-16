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


### FFT's Explained:
Besides Amplitude vs Time, we also would need an analysis of the frequencies that occur in the music file. This is what FFT (Fast Fourier Transform) is for. In short, a Fourier Transform (there are many types of them) changes an Amplitude Domain to a Frequency Domain. 

This is where the 2nd part of the code comes in (as shown below):

![image](https://github.com/user-attachments/assets/c836d9d4-7919-4c80-99a0-fd5d0268b305)

### A couple of things to explain:
1.) An FFT will render data from Amplitude vs. Time --> Magnitude vs. Frequency

2.) fft = np.fft.fft(signal) feeds the signal into a fft 

3.) magnitude = np.abs(fft)

4.) frequency = np.linspace(0, sr, len(magnitude))

5.) 

6.) Lastly, you are updating the plot to contain the transformations that were conducted above. And you should get a graph that looks something like this:

![image](https://github.com/user-attachments/assets/9a2a6274-d8b3-451b-a7bb-6bf79cb8cb72)
