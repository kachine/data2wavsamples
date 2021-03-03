# data2wavsamples
samples and TX16Wx programs by data


## What's this
This repository contains:
- Loopable wave files
- Programs for TX16Wx


### Loopable wave files
The wave files in this repository are designed for small footprint, to use with loop function in sampler.
And it has embedded loop markers.
Sampler software which supports "smpl" chunk will recognize the loop information such as loop points and root note (Tested with DirectWave in FL Studio).

If your sampler does not recognize loop information, you should manually specify loop range from start to end of waveform (i.e. entire waveform).


### Programs for TX16Wx
The *.txprog files is for TX16Wx sampler software.
TX16Wx has some data file, *.txprog is a program file.

At the point of initial commit, *.txprog is very basic setting like below:
- Fast attack time
- Fast release time
- BiQ LPF (cutoff frequency: 20KHz) for eliminate aliasing noise
- SVF HPF (cutoff frequency: 20Hz) for eliminate DC noise


## Some information
- These small wave files should not be compressed with FLAC. The file size will be increased.
- The original waveform was taken from some data, such as room temperature. Then, the wave table sound engine ("波形メモリ音源" in Japanese) generates a specific frequency waveform.
