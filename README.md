# 💡 SETUP

## Required Files:

#### music/ (folder for all song files, .wav only, no spaces in the name) 
#### titles/ (input videos that are LONG - only for long intro /outro songs, .mp4 only)
#### videos/ (all other input videos, .mp4 only)

## ⚫ INSTALL DEPENDENCIES FROM A CONDA ENVIRONMENT (strongly reccommended)

### make and activate new conda environment

```conda create -n [myEnv]```
```conda activate [myEnv]```

### navigate to the MusicVideoGenerator folder then run

```conda install --file Requirements.txt```
```pip install -r Requirements2.txt```

# 🟢 USEAGE:
 
```python MusicVideoGenerator.py -songName [song.wav] -bpm [int] --output [outputPrefix] --dynamic [True/False]```

# 🛑 FAQS:

## What does it do?

- This program cleverly assembles your previously downloaded scaffold videos into a tempo synced music video based on a provided input song and bpm

## How does it do it?

1. Analyses a .wav file (located in music/)
2. Generates 3 seperate tempo and dynamically synced music videos out of random .mp4 videos located in videos/
3. Combines them through the use of overlay FX into one video located in output/ 
4. Applies chroma shifting to the final product to make the videos bleed into eachother for contrast.  

## What does "dyamically synced" mean?

- Louder sections of your input song have a higher chance of faster / more intense visuals and vice versa.

## What does it not do?

- Generate music videos from thin air.

## Where can I find sample videos to use?

Royalty Free:
- https://www.pexels.com/
- https://pixabay.com/

There are also a small selection of videos in this repo to allow you to test the program. These are from pexels.  

## What is the ouput format?

- Video is 720p, audio is 256kps AAC

## How fast is my song? What is my songs BPM?

- https://www.beatsperminuteonline.com/
