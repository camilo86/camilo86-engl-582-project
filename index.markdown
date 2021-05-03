---
layout: home
---

> **Note:** Project still in review

# Analysing the effectiveness of denylist, sentiment analysis and text classification in hate speech detection

By: Camilo Gonzalez ([cxg7732@rit.edu](mailto:cxg7732@rit.edu))

## Intro

In this project, I will be assessing three standard methods of hate speech detection (denylist, sentiment analysis, and
text classification). I will be running each detection method through a dataset to understand their performance at
detecting hate speech and how they stack up against other existing methods.

Using these results, I hope to shine some light into the effectiveness of these systems, and hopefully find ways in
which these systems can be leveraged to be more powerful at identifying different types hate speech online.

## Motivation

Social media has made our world smaller. With a push of a button, you can share your thoughts with millions of
people all around the world. Unfortunately, the same technology that has brought us together is also being used to
amplify hate, disinformation, and to radicalize.

Although the tech sector is aware of the hate speech problem, and is actively building new tools to mitigate the
issue, the current methods are not enough.

## Method

I will build and assess three methods of hate speech detection:

- Denylist of common hate speech words
  - [Popular denylist used and mantained by Shutterstock](https://github.com/LDNOOBW/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words)
- Sentiment anylisis (VADER)
  - NLTK’s VADER for social media sentiment anaylysis
  - [Trained using pre-labeled dataset](https://github.com/ZeerakW/hatespeech)
- BERT Text classification

Once these three systems are built, I will test each system against a dataset that contains both [hate and non-hate
speech](https://github.com/t-davidson/hate-speech-and-offensive-language)

## Experimental Design

I will record how each system classified each word in the dataset and compare it against the actual hate-speech label
in the dataset. I will calculate how many words were classified correctly, false positives and false negatives.

Once the data is collected, I will be able analyse the results and answer the following questions:

- Which system performs best overall?
- What categories of hate speech were easiest/hardest to categorize overall?
- Are any of these systems better at identifying a specific type of hate speech than others? If so, why?

## Data

There are a few datasets needed to create the three systems and to test them.

- [”List of dirty naughty obscene, and otherwise bad words” set will be used as the denylist for the first system.
  This list is very popular and has already been integrated in Overstock application for image label review and
  into many open source tools for developer](https://github.com/t-davidson/hate-speech-and-offensive-language)
- [”Hateful people or hateful symbols” set will be used to create the text classifier system. This dataset is
  composed of problematic tweets along with user profile name and bio, and was published by the Association
  for Computational Linguistics](https://github.com/ZeerakW/hatespeech)
- [”Hate speech and offensive language” set will be used to test each of the three systems. This set contains
  text extracted from problematic tweets and Facebook posts, and was presented in the proceedings of the
  11th Internation AAAI conference on web and social media](https://github.com/t-davidson/hate-speech-andoffensive-language)
