# WatchWise-Content-Based Movie Recommender System

This project implements a content-based movie recommender system using movie tags and a neural network. The system is designed to recommend movies based on their similarity in terms of tags associated with them.
Watchwise is the movie recemmonder system based on TMDB 5000 Movie Dataset
I have used movies and an attribute called tags containing list of cast, genre, 
Watchwise uses auto encoder type architecture to obtain embeddings 

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Model Used](#Model_Used)

## Introduction

The recommender system uses a multi-label binarizer to encode movie tags into binary vectors. It then trains an autoencoder neural network to learn a compressed representation (embedding) of these tags. The embeddings are used to find and recommend movies that are similar based on their tag representations.

## Prerequisites

- Python 3.6+
- PyTorch
- scikit-learn
- NumPy
- Pandas

## Model_Used
The neural network used in this content-based movie recommender system is an autoencoder. Let's delve into what an autoencoder is and how it is used in this context.

Autoencoder Overview
An autoencoder is a type of artificial neural network used to learn efficient representations of data, typically for the purpose of dimensionality reduction or feature learning. The network architecture consists of two main parts:

Encoder: This part compresses the input data into a lower-dimensional representation, known as the latent space or embedding.
Decoder: This part reconstructs the input data from the lower-dimensional representation.
The goal of the autoencoder is to reconstruct the input as accurately as possible, thus forcing the network to learn the most important features of the data.
