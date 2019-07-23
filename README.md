# Production Feedback Tool

This is a tool to give online feedback on vowel production, using the computer program Praat (Boersma & Weenink, 2016). 
It can be used to analyze and give visual feedback on productions of the English /ɛ/–/æ/ contrast, to train the pronunciation of this contrast for non-native English speakers.

The current version of the tool is only available for female speakers. If you would like to use the tool for male speakers, you can open an issue to request this.

## Background
This tool can be used to train speakers’ production of a non-native vowel contrast. Tools to do this kind of training have been developed (for a review see Kartushina et al., 2015, JASA, 138(2), 817-832), but are not open-source. Moreover, most training studies do not explicitly test whether the dimensions the tool uses for feedback are optimally informative/relevant for learning the contrast. The studies mentioned in Kartushina et al. (2015) differ greatly in terms of behavioral improvements as well as in terms of the methods of the studies. Feedback systems are different, and different acoustic measures are used. There thus seems to be inconsistency in the features that are used to base the feedback on, which means that some studies might give feedback based on features that are not so relevant in speech perception, or they leave out important features. 

For this tool, we carried out an extensive linear discriminant analysis (LDA) to analyze a dataset of productions of the our vowels of interest (the English /ɛ/ in ‘pen’  and /æ/ in ‘pan’), produced by 10 native speakers of English. We did this to identify the most important features of the English vowels /ɛ/ and /æ/ were identified, because these features will be most useful to receive feedback on for non-native speakers. We found mean F1 and F2 over the whole duration of the vowel are the best indicators, and that coarticulation should be taken into account. Our tool thus uses these features to provide the participant feedback on her vowel production. More information on how the tool was developed can be found [here](thesis-GiselaGovaart.pdf).

## The tool
The tool consists of:
- Training 1: Feedback training (the participant produced the words and gets visual feedback on her pronunciation) 
- Training 2: Control training (same as training 1, but without visual feedback on own production)
- Transfer Reading: A transfer reading task with 8 new words.
For Training 1 and 2, if session number = 1, the training starts with a practice phase with 20 words. The transfer reading task does not have a practice phase.

The script test_axes_females.praat was used to decide the values of the axes. To see the distribution of the means of the vowels in the five different consonant contexts, see have a look this script.

## Using the tool
Information for experiment leader:
- After the initial calibration phase, you should check whether the three vowels are on a triangle, and whether the values make sense. If the triangle does not look good, redo the calibration, because this influences all vowels in the experiment.
- When the experiment is finished and you see the last screen, press the space bar one last time. Do not just close the window by pressing the cross in the left-top corner – the window closes by itself after you press the space bar.

## Collaborators
- Gisela Govaart
- Makiko Sadakata
- Paul Boersma

This tool was created as part of a research internship at the Donders Institute, Nijmegen and the Amsterdam Center for Language and Communication: Phonetic Sciences, Amsterdam. 

We thank: Jana Thorin, Dirkjan Vet, James McQueen, David Weenink, Peter Desain
