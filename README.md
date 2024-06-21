# Anim-400K: A dataset designed from the ground up for automated dubbing of video
Official repository for the Anim-400K dataset. [[ArXiv Preprint](https://arxiv.org/abs/2401.05314)]

![image](https://github.com/DavidMChan/Anim400K/assets/3190178/d819fc8c-2e56-4ed0-bf3a-1b249899cbdc)

# What is Anim400K?

Anim400K is a large-scale dataset of aligned audio-video clips in both the English and Japanese languages. It is comprised of over 425K aligned clips (763 hours) consisting of both video and audio drawn from over 190 properties covering hundreds of themes and genres. Anim400K is further augmented with metadata including genres, themes, show-ratings, character profiles, and animation styles at a property level, episode synopses, ratings, and subtitles at an episode level, and pre-computed ASR at an aligned clip level to enable in-depth research into several audio-visual tasks.

# News
**[January 2024]** Anim400K (v1) available on [Huggingface Datasets](https://huggingface.co/datasets/davidchan/anim400k). </br> 
**[January 2024]** Anim400K (v1) release. </br>
**[January 2024]** Anim400K (v1) accepted at ICASSP2024. </br>

# Request access to the Anim400K dataset

We provide two means of getting access to the dataset:

## Option 1: Huggingface Datasets

To get access to the Anim400K dataset (annotations and clips) please follow these steps:

1- Log into your Huggingface account, and fill out the dataset request form [here](https://huggingface.co/datasets/davidchan/anim400k)

2- Use the Huggingface CLI/tools to download the data. The tar.gz files are provided as .tar.gz-part files, which need to be assembled before unzipping. This can be done following the instructions [here](https://askubuntu.com/questions/1179657/how-to-extract-tgz-part).

## Option 2: Email

To get access to the Anim400K dataset (annotations and clips) please follow these steps:

1- Complete this form ([link](https://forms.gle/7xBp2uFP4Fb4UZye9)) and sign the TOU (Terms of Use) and NDA (Non Disclosure Agreement).

2- We will verify the correctness of the provided information. 

3- You will receive an email with the links and information to download the data.

See the data documentation [here](doc/README.md).


# Citation
If any part of our paper is helpful to your work, please cite with:
```
@inproceedings{cai2024anim400k,
  title={ANIM-400K: A Large-Scale Dataset for Automated End to End Dubbing of Video},
  author={Cai, Kevin and Liu, Chonghua and Chan, David M.},
  booktitle={ICASSP 2024-2024 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
  pages={1--5},
  year={2024},
  organization={IEEE}
}
```

# Acknowledgements

The Github repository, and data release model is modeled on that used by the [MAD](https://github.com/Soldelli/MAD) dataset. 
