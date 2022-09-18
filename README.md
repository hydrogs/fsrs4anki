# fsrs4anki

The fsrs4anki is an Anki [custom scheduling](https://faqs.ankiweb.net/the-2021-scheduler.html#add-ons-and-custom-scheduling) implementing the scheduling module of [Free Spaced Repetition Scheduler algorithm](https://github.com/open-spaced-repetition/free-spaced-repetition-scheduler). The adaptive module is developed in Google Colab.

Supported Anki version >= 2.1.55 (related discussion: [Some problems in implementing a state-of-the-art SRS scheduler on Anki - Scheduling - Anki Forums (ankiweb.net)](https://forums.ankiweb.net/t/some-problems-in-implementing-a-state-of-the-art-srs-scheduler-on-anki/22705))

## Usage

> Remember to use the dev version of Anki because the customData feature was implemented in the last two weeks. It has not been released yet.

Please copy the code in [main.js](main.js) and paste it into the bottom of the deck options screen (need to enable the scheduler v3 in Preferences), then it works.

![deck options](images/deck_options.png)

## Optimization

The default parameters of fsrs4anki are trained from my review logs. If you want the algorithm more adaptive to you, please follow the guide in [fsrs4anki_optimizer.ipynb - Colaboratory (google.com)](https://colab.research.google.com/drive/1pCg1KesWy7dD4Gu7BcBqY2thw370JZTk?usp=sharing). The exemplary process is recorded in [fsrs4anki_optimizer.ipynb at main · open-spaced-repetition/fsrs4anki (github.com)](fsrs4anki_optimizer.ipynb).