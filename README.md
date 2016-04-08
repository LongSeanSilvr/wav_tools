# wav_merge.py
A tool for merging all .wav files within a given directory. A bit quicker than merging multiple .wav files in Praat,
and a hell of a lot quicker than merging .wav files using Audacity.

* USAGE: (python) wav_merge.py \<directory_name/path/>

* SETUP: 
  * This program debends on pydub. To install this package, enter the following command in a terminal:  
  ``` pip install pydub```

* NOTES:
  * NAME ALL FILES SO THAT THEY AUTOMATICALLY SORT CORRECTLY. This generally means name all files the same except for 
  an ordering number suffix (e.g. "myfile_01, myfile_02, ...")
  DO NOT forget to put zeros before single digit part numbers, or this script 
  will merge files in the following order: "file_1, file_10, file_11, file_2, file_3, file_4, ..., file_9"
  * Requires either that the directory to be merged is under the same directory as the script itself, or that an 
  absolute path to the directory to be merged be specified.
  * Stores the resulting .wav file as "combined.wav"
  * Currently only compatible with Windows operating systems.

