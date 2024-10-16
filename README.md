# Dissecting-Spotify-Valence

## Introduction

Spotify uses a metric called *valence* to measure the happiness of a track. The metric itself, however, was not developed by Spotify. It was originally developed by Echo Nest, a company that was bought by Spotify in 2014. We don't know exactly how valence is calculated. Some details are given by a blog post, which you can find here:

https://web.archive.org/web/20170422195736/http://blog.echonest.com/post/66097438564/plotting-musics-emotional-valence-1950-2013

The goal is to untangle the mystery behind valence and propose how this is derived.

Spotify offers the following information:

* [Get Track's Audio Features](https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-features) and [Get Tracks' Several Audio Features](https://developer.spotify.com/documentation/web-api/reference/#/operations/get-several-audio-features).

* [Get Track's Audio Analysis](https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-analysis).

## Data

* The data utilised for the models came from 2 sources: [Kaggle](https://www.kaggle.com/datasets/zaheenhamidani/ultimate-spotify-tracks-db?resource=download) and [Zenodo](https://web.archive.org/web/20170422195736/http://blog.echonest.com/post/66097438564/plotting-musics-emotional-valence-1950-2013). 
* The IDs of the songs contained in the previously mentioned datasets were passed through Spotify's API to acquire their features which were then written in a file called `tracks.csv`.
* `tracks.csv` was very large for GitHub so instead a sample was uploaded called `sample_tracks.csv`.

## Objectives

1) Understand the influence of various track features on valence.
2) Predict valence based on track features.

<img width="460" alt="spotify-logo-transparent-high-resolution-4-1544236771-1" src="https://github.com/user-attachments/assets/7763b273-3444-4c93-982c-5bc60ec9a77f">



