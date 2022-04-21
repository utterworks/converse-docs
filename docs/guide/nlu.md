# Natural Language Understanding

The Natural Language Understanding section is where intents, entities and training data are maintained. Technology plays a major role, but the most significant performance gains are obtained by developing a good understanding of the fundamental NLU concepts.

## Intents
An intent captures the general meaning of a sentence (or an utterance in the chatbots lingo). For example, the sentences below convey the intent of being hungry, let’s call it i_am_hungry:

I am hungry
I need to eat something
I am starving
My kingdom for a pizza
How do we teach our model that these utterances convey the i_am_hungry intent? We train it to distinguish them from sentences with other meanings. We create a dataset containing examples of different intents.

How can a program understand the meaning? Let’s just say that there’s a way to express the meaning of words with numbers (or vectors). The essential idea is that vectors can be compared (a distance can be calculated), and that a small distance indicates the words have similar meaning.

When you click the Train button, Rasa, the conversational AI framework used by Converse, will learn vectors from your examples, and learn how to distinguish intents.

Use the Intent section to maintain the list of intents the project supports. Additional attributes for an intent can also be maintained here, as well as details of the training data associated with the intent and a link to that training data.

There are some default system intents that come pre-created - these include common conversational intents like affirm and deny, don't know and explain. These are often used in slot extraction or validation as will be covered later in this guide

## Entities
If an intent carries the general meaning of a user utterance, sometimes you need additional information. Consider the following utterances:

I want to buy a blue shirt
I want to buy a red short
In both cases, the intent is to buy something. The color is a useful information, but we don’t want to have a different intent for each color.

The color is an additional information to extract and that’s a perfect candidate for an entity - Entities are elements you want to extract from a user utterance.

> The platform containes a number of built in entities that are available for use in things like slot extraction. These built in entities include things like time, distance, number, email address

==Additional custom entities can be created, these can be simple regular expressions, or they can be more complex concepts that the platform can be trained to recognise==

## Training Data
The NLU recognises intents by being given examples from which it can generalise. Training data for intents is added in the Training Data section. This training data can also be used to identify and train entities too. 

## Trained Entities
To add trained entities must teach the platform how and where to find these entities in your utterances. You can do this by tagging entities in the user utterances you provide as examples in the training data section.

