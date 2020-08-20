# Emoji Prediction

## Table of Contents (Optional)
---
- [dataset](#dataset)
- [sample_data](#sample)
---

# dataset
- you'll find dataset in dataset folder
- it consist of sentences and correspond a number which describes emoji

# sample
- `emoji_dictionary = {"0": "\u2764\uFE0F",    # :heart: prints a black instead of red heart depending on the font
                    "1": ":baseball:",
                    "2": ":beaming_face_with_smiling_eyes:",
                    "3": ":downcast_face_with_sweat:",
                    "4": ":fork_and_knife:",
                   }`
- `for e in emoji_dictionary.values():
    print(emoji.emojize(e)) ` 
- **output**
- ❤️
- ⚾
- 😁
- 😓 
- 🍴


### This is the sentance with label output
- never talk to me again 😓
- I am proud of your achievements 😁
- It is the worst day in my life 😓
- Miss you so much ❤️
- food is life 🍴
- I love you mum ❤️
- Stop saying bullshit 😓
- congratulations on your acceptance 😁
- The assignment is too long  😓
- I want to go play ⚾

---

> PreProcessing


- first convert it into one hot encoding
- then using glove vector convert words into embeddings
- then make a model using LSTM layers 
- compile the models 
- fit the model 
- get the prediction   
