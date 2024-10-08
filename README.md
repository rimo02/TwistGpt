﻿# TwistGpt

![alt text](assets/gpt2.png)

This repository contains the implementation of GPT-2 pretraining from scratch using the short stories of O. Henry, known for their surprising endings. Due to resource constraints, the model couldn't be trained for multiple epochs, but efforts were made to minimize the model's loss.

# Data

The data can be found in the `final.txt` file which has been prepared by scraping using python script `scrape.py`. Remember to put `<|endoftext|>` at the end of each desired para that marks the beggining of a story. This is essential for the model to better understand the context behind.

# Training

1. You can create your own dataset to train and prepae a `.txt` file accordingly.
2. Install the dependencies in `pip install -r requirements.txt`
3. Get inside the `src` directory and then run `python train.py`.
   The model should start running without any errors

# Testing

To test your model performance, call the `inference.py` and pass any prompt
I have given the prompt as- Passing by the subway, and the result i got

`Passing by the subway                    
Lord Oakhurst was thinking of life and worked out and st toward the avenue. And now rushed out of the window and the softness in sweet, and deliberate, proclaimed that led the doorway to the great tourney, and to the great iron gates of the park. Lord Oakhurst had been a great sportsman during his life and always kept a well-stocked kennel of curs, which now rushed out from their hiding places and with loud yelps sprang upon the physician, burying their fangs in his lower limbs and seriously damaging his apparel.
Sir Everllard, startled out of his professional dignity and usual indifference to human suffering, by the personal application of feeling, gave vent to a most horrible and blighting CURSE and ran with great swiftness to his carriage and drove off toward the city.
<|endoftext|> `

### Reference

- [Andrej Karpathy](https://github.com/karpathy/minGPT)
- [WillyGPT](https://github.com/nikhil-xb/WillyGPT)
