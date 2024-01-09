# Anim400K: A dataset designed from the ground up for automated dubbing of video

## Introduction
Official repository for  Anim400K. [[ArXiv Preprint]()]

Paper accepted @ICASSP2024. 

![image](https://github.com/DavidMChan/Anim400K/assets/3190178/d819fc8c-2e56-4ed0-bf3a-1b249899cbdc)


# News
**[January 2024]** Anim400K (v1) accepted at ICASSP2024. </br>
**[January 2024]** Anim400K (v1) release. </br>



# What is Anim400K?

Anim400K is a large-scale dataset of aligned audio-video clips in both the English and Japanese languages. It is comprised of over 425K aligned clips (763 hours) consisting of both video and audio drawn from over 190 properties covering hundreds of themes and genres. Anim400K is further augmented with metadata including genres, themes, show-ratings, character profiles, and animation styles at a property level, episode synopses, ratings, and subtitles at an episode level, and pre-computed ASR at an aligned clip level to enable in-depth research into several audio-visual tasks.


# Request access to the Anim400K dataset
To get access to the Anim400K dataset (annotations and pre-extracted features) please follow these steps:

1- Complete this form ([link](https://forms.gle/7xBp2uFP4Fb4UZye9)) and sign the TOU (Terms of Use) and NDA (Non Disclosure Agreement).

2- We will verify the correctness of the provided information. 

3- You will receive an email with the credentials to download the data.

See the data documentation [here](doc/README.md). 



# Data Download
The confirmation email will contain LINK and PASSWORD to access the data. Each file can be downloaded from the web interface or through the provided script `Anim400K_downloader.py `, which can be used as follows:

```bash 
python Anim400K_downloader.py --destination_folder {PATH_TO_DOWNLOAD} --download_link {LINK} --password {PASSWORD} 
```

Required Dependencies: `pip install tqdm minio`


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
