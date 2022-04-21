# Project-3

## Abstract

Project Three: Tutorial Prototype details the process of designing spaCy tutorials for the Scholars Studio website. This plan analyzes user needs for successful tutorials and aims to create tutorial prototypes that address those needs. The tutorials featured in this plan revolve around Named Entity Recognition (NER) and tokenization. The publication objectives of these tutorials go through each prototype and explain what goal of the publication is and how it successfully meets those goals. These tutorials are broken down into specific explanations of why each design choice was made and how these decisions benefit the user experience. Moreover, these tutorials demonstrate how previous other tutorials can implement the needs of users to successfully teach the desired content. The conclusion analyzes the needs the tutorial needed to address and how the tutorials addressed them effectively.

## Purpose of Project

Produce intro level tutorials for Temple students, employees, and faculty on the usage of spaCy, Google Colab, and Github. 

## Purpose of Documentation

To draw attention to the Scholars Studio website and create an archive of tutorials to be managed by the Scholars Studio staff.


## Audience Profile

The users of these tutorials come from a variety of backgrounds with different levels of experience. This diversity ranges from experienced users who are looking for supplemental material in their programming class to people who are completely unfamiliar with any coding and are trying to teach themselves for the first time. With that in mind, it’s important to keep the content accessible to all users regardless of how familiar they are with the content.

When observing the small sample size within this class it’s clear that certain types of tutorials do not work for everyone. One of the largest barriers to entry is the amount of vocabulary and technical jargon that gets used casually within these tutorials that lack explanation. Moreover, I’ve seen others struggle with how the tutorials are organized and what exactly is expected from the user. Others, with perhaps a bit more experience, find certain aspects of the tutorials to be confusing. For instance, a tutorial will explain to users how to find named entities from a series of imported sources but will fail to explain how they imported the sources to begin with. This makes the tutorial impossible to replicate for any other type of information without the user having to look up a completely separate tutorial for that initial step.

This perhaps leads into the most challenging aspect of tutorials, which is: how much information should be included? It’s obvious that when designing for users who may be complete beginners a lot of information is necessary that might be more obvious to experienced users. Moreover, if a tutorial overwhelms the user with too much information then it could lead to a negative user experience. There is a very precise balance that needs to be met in order for these tutorials to be effective for all users.

## Usability Goals

A series of tests were conducted to discover users’ experience with various tutorials. These tests were aimed to find what methods were effective in teaching users and which were detrimental to their learning (Hackos, 1994). Users were asked to follow tutorials with interactive components versus non interactive tutorials. Additionally, there was special attention given to the amount of information– how much was necessary and at what point did it become too much information for the user to sift through to get to the desired content. Finally, these tests aimed to figure out which layout design worked best for users’ needs. 

## Publication Objectives

### Named Entity Recognition Tutorial:

My Named Entity Recognition (NER) is a tutorial designed around teaching the basics of what Named Entity Recognition is. This begins with a basic overview of what spaCy is followed by various terminology relevant to the material being taught. I think defining terms like `Doc` `Token` objects and `NER` were vital for new users to learn the material. This is followed by a table that lists out every single entity, followed by the abbreviation spaCy uses, the entity definitions, and various examples of what that entity would identify. I felt like this table was an invaluable resource as it allows users to clearly see all the entities spaCy has to offer as well as what they are. By having this information clearly laid out in a table format users are able to compare and contrast different entities and easily refer back to the chart if there is ever confusion. The table also helps define terms and technical terminology as later in the tutorial various entities are identified but through the use of the spaCy abbreviation. New users will be unfamiliar with terms like `LOC` or `GPE` so having a chart defining the terms they will encounter using NER is important. Afterwards there is an interactive element where users can input their own text and see how spaCy would label various entities. This interactivity of this element allows for user interaction while not leaving room for user error if they potentially execute a code wrong; moreover, this section also allows users to find more examples of entities that may be confusing and allow them to get further clarification of how spaCy works. The rest of the tutorial addresses the various uses and potential pitfalls of using NER. It demonstrates the various results NER can have such as splitting up one entity into multiple tokens or keeping the whole entity together. It also explains why certain usages might be confusing or less desirable than others. This tutorial is designed to be a basic overview for beginners trying to learn what a Named Entity is and why they are relevant.



### Tokenization Tutorial:

#### Overview:

The other tutorial I created is designed to teach tokenization as well as the differences between digits and numbers in spaCy. Much like the NER tutorial, this tutorial also features a brief definition of what spaCy is as well as other relevant terminology. This might be repetitive, but I wanted to design the tutorials to be able to stand on their own; I didn’t want to assume that users have already looked at one tutorial before looking at the other. This is why they both feature the same overview. It then goes on to explain the token attributes the tutorial is teaching and what they would identify– digits and numbers. Overall this tutorial is much longer than the NER tutorial and is broken into three sections increasing in difficulty. These sections are then followed by an opportunity for users to practice what they’ve learned. A solution is also provided to ensure users have gotten the correct answer as well as an explanation of why the correct answer is correct. I used the explanation to address some of the more common confusions I’ve seen arise from user testing. While I have redesigned the tutorial to address most of these issues upfront, there are still a few things I think can’t be necessarily addressed in the tutorial itself without cluttering the content and becoming information overload. Moreover, these minor issues are something inexperienced users will probably encounter initially but are able to work through. An example would be when the tutorial asks users to process a specific text: users will often look back to the example and simply copy and paste the code from the “Process the text” step without changing the name of the code they are processing. In the practice problem the text is called “example” whereas in the tutorial the text the tutorial uses is just referred to as “text”. Users are able to rectify this issue on their own usually, but the solution also addresses this common mistake in the event they are unable to. The solution is also helpful to users who get the correct answer as it provides more explanation of what specifically is correct about the answer they input.

#### Section One:

The first section is designed to teach users how to find both digits and numbers within a text. It explains why a user would want to use these two attributes as well as highlights the differences between the two. This section is fairly basic and features a practice problem that is fairly identical to the tutorial itself. This practice problem isn’t designed to be challenging, it’s just to reinforce the learning as well as highlight common mistakes new users might make such as processing the text wrong as discussed previously.

#### Section Two:

The section offers a more relevant use case, which is siphoning out all the numbers and digits from a body of text. The tutorial then shows how these numbers and digits can be put into their own list and printed out. This section once again highlights the differences between the two attributes and explains why they cannot be used interchangeably. If someone used the like.digits attribute attempting to find any numerical value they would be misled because the like.digits attribute doesn’t identify numbers written out as words or any number that features punctuation such as a comma or period. This section is once again followed by a practice problem that asks users to expand upon the previous exercise. While a little more complex, this problem should still be manageable for new users to complete with the aid of the tutorial. Once again a solution and explanation is provided.

#### Section Three:

This section is the most advanced as it once again builds off the previous section. In this section users are shown a different use case scenario, which is removing digits and numbers from a body of text. This is done through a multi-step for-loop as opposed to the single step for-loop used in section two. This for-loop is explained in great detail showing what exactly is being done and how it gets the results. This is followed by the same code without the comments so users are able to copy and paste for their own usage without having to delete the various comments and risk ruining the format. This section also explains how to remove digits from a list of numbers once again using a multi-step for-loop with various conditions. This section addresses what is perhaps the most useful way like.digits can be used since up to this point the like.digits attribute has only been shown to be a less helpful version of like.num. This section is the most advanced and requires the most explaining as new users are probably unfamiliar with multi-step for-loops and multiple conditional statements. This is once again followed by a practice problem where users are asked to make a list with numbers without digits. This practice problem resembles the previous problems but with greater complexity. Users should be able to use the tutorial and get the solution on their own, but there is once again a solution and explanation to provide further clarification.

## Conclusion

These tutorials meet the needs of the audience by being explanatory without an abundance of information. Moreover, the terms and structure of the tutorials are kept consistent so users can focus on the content rather than be distracted by trying to understand the layout. The tutorials address common user needs and provide a plethora of opportunities for user learning. This is done through exploratory learning as demonstrated with the interactive element of the NER tutorial as well as knowledge testing such as the practice problems in the tokenization tutorial. These tutorials are also clear, concise, and leave little room for user error. Additionally, by being designed for new users, this makes the tutorial accessible to anyone wishing to learn coding, not just those who are already familiar with it. The informational sections are broken down into short easy to follow steps and further explanations can be found at the user’s pace. I believe these tutorials successfully teach the topics they’re designed for to the intended audience.

## References
Hackos, J. A. T. (1994). *Managing your documentation projects.* John Wiley & Sons.
Shrivarsheni. (2021, May 27). Spacy tutorial - learn all of spacy in one complete writeup: 
ML+. Machine Learning Plus. Retrieved March 21, 2022, from https://www.machinelearningplus.com/spacy-tutorial-nlp/

*Spacy 101: Everything you need to know · spacy usage documentation.* spaCy 101: 
Everything you need to know. (2016). Retrieved March 21, 2022, from https://spacy.io/usage/spacy-101/
