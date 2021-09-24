# TV-Script-Generation-RNN

## Introduction
In this project, you'll generate your own <a href="https://en.wikipedia.org/wiki/Seinfeld">Seinfeld</a> TV scripts using RNNs. You'll be using a <a href="https://www.kaggle.com/thec03u5/seinfeld-chronicles#scripts.csv">Seinfeld dataset</a> of scripts from 9 seasons. The Neural Network you'll build will generate a new, "fake" TV script, based on patterns it recognizes in this training data.

## Generate TV Script
With the network trained and saved, you'll use it to generate a new, "fake" Seinfeld TV script in this section.

## Generate Text
To generate the text, the network needs to start with a single word and repeat its predictions until it reaches a set length. You'll be using the generate function to do this. It takes a word id to start with, prime_id, and generates a set length of text, predict_len. Also note that it uses topk sampling to introduce some randomness in choosing the most likely next word, given an output set of word scores!

## Result
You will see that there are multiple characters that say (somewhat) complete sentences, but it doesn't have to be perfect! It takes quite a while to get good results, and often, you'll have to use a smaller vocabulary (and discard uncommon words), or get more data. The Seinfeld dataset is about 3.4 MB, which is big enough for our purposes; for script generation you'll want more than 1 MB of text, generally.
