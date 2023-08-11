
AI Pokedex 

An AI Pokedex designed to accurately identify 108 different pokemon 

![Abra Screenshot 2023-08-10 125534](https://github.com/dmcneroforte/Pokedex/assets/141778017/447e6bd2-5de8-4eae-afbe-687063770b11)

## The Algorithm


The AI Pokedex is utilises imagenet, which is code required to accurately identify an object in a photo, for this specific project 108 classes of pokemon were transfered from the computer onto the jetson nano developer kit, this was so the jetson nano could be trained to identify each pokemon through the usage of downloading epochs. An epoch is the name for one passing of training data within the jetson nano. The more epochs are downloaded the more accurate the jetson nano becomes in the context of identifying pokemon. This project required a pre trained resnet18 model that was then trained further in order to accomadate the needs of the project, identifying each pokemon


## Running this project

In order to run the project, the model would have to be on the jetson nano, in order to check if the model is on the nano, you would have to input the command “Is models”. What this does is list the available models, having done this you should be able to see resnet18.onx. You would then need to set the NET and DATASET variables by using the code “NET-models” and “DATASET=data.” Having done this, the next command that needs to be run is “magenet, imagenet.py model-$NET/resnet18.onx —input_blob-input_0 —output_blob=output_0 _ - labels-$DATASET/labels.txt $DATASET/test/Abra/01.jpg Abral. jpg” This command is necessary to identify a specific Pokemon according to context. Within this context, the pokemon that is being assessed for identification is “Abra”, specifically the first image available depicting “Abra”. Having done this, the AI will provide a percentage indicating how
“confident” it was in its conclusion. For example,
“87% Abbra”. This
You sent
would mean that the AI is 87% sure that the image provided was in fact
“’Abra’


[View a video explanation here](video link)# Pokedex


https://github.com/dmcneroforte/Pokedex/assets/141778017/6b7ccf01-7ea9-473d-abf9-fccd183c6a65

