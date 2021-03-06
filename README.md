# IQ_Research

That is our research on Vocabulary IQ done in R to find some correlations between IQ and biography status or random facts.

In order, to see what I have done - check Research directory. The pdf version is the best displayable.

Authors:
* [Taras Svystun](https://github.com/taras-svystun)
* [Dmytro Kalitin](https://github.com/just1ce415)
* [Yaroslav Tsymbalista](https://github.com/agravitybrain)

Link to the original database and its description is [here](https://www.kaggle.com/yamqwe/vocabulary-iq-test)

## Data description
This data was collected on-line through an interactive test titled "Vocabulary IQ Test" between July 2017 and March 2018. 

The main body of the test had 45 vocabulary questions. Each question was a list of five words. Subjects were instructed to select the two on the list that had the same meaning. Subjects were also instructed to not guess and were told there was a -0.35 point penalty for a wrong answer.

Calculated scores are availible in these three variables:

score_right	Number of questions that were answered correctly.

score_wrong	Number of questions that were answered incorrectly.

score_full	= score_right - 0.35 * score_wrong.


Below are the words used for the questions with the correct answers for each question:

## IQ questions
item	answer	words

Q1 	24 	tiny faded new large big

Q2 	3 	shovel spade needle oak club

Q3 	10 	walk rob juggle steal discover

Q4 	5 	finish embellish cap squeak talk

Q5 	9 	recall flex efface remember divest

Q6 	9 	implore fancy recant beg answer

Q7 	17 	deal claim plea recoup sale

Q8 	10 	mindful negligent neurotic lax delectable

Q9 	17 	quash evade enumerate assist defeat

Q10 	10 	entrapment partner fool companion mirror

Q11 	5 	junk squeeze trash punch crack

Q12 	17 	trivial crude presidential flow minor

Q13 	9 	prattle siren couch chatter good

Q14 	5 	above slow over pierce what

Q15 	18 	assail designate arcane capitulate specify

Q16 	18 	succeed drop squeal spit fall

Q17 	3 	fly soar drink peer hop

Q18 	12 	disburse perplex muster convene feign

Q19 	18 	cistern crimp bastion leeway pleat

Q20 	18 	solder beguile distant reveal seduce

Q21 	3 	dowager matron spank fiend sire

Q22 	18 	worldly solo inverted drunk alone

Q23 	6 	protracted standard normal florid unbalanced

Q24 	12 	admissible barbaric lackluster drab spiffy

Q25 	17 	related intrinsic alien steadfast pertinent

Q26 	10 	facile annoying clicker obnoxious counter

Q27 	10 	capricious incipient galling nascent chromatic

Q28 	9 	noted subsidiary culinary illustrious begrudge

Q29 	9 	breach harmony vehement rupture acquiesce

Q30 	3 	influence power cauterize bizarre regular

Q31 	6 	silence rage anger victory love

Q32 	10 	sector mean light harsh predator

Q33 	17 	house carnival yeast economy domicile

Q34 	3 	depression despondency forswear hysteria integrity

Q35 	17 	memorandum catalogue bourgeois trigger note

Q36 	24 	fulminant doohickey ligature epistle letter

Q37 	17 	titanic equestrian niggardly promiscuous gargantuan

Q38 	5 	stanchion strumpet pole pale forstall

Q39 	5 	yearn reject hanker despair indolence

Q40 	24 	introduce terminate shatter bifurcate fork

Q41 	5 	omen opulence harbinger mystic demand

Q42 	5 	hightail report abscond perturb surmise

Q43 	12 	fugacious vapid fractious querulous extemporaneous

Q44 	10 	cardinal pilot full trial inkling

Q45 	9 	fixed rotund stagnant permanent shifty



The given answer is an integer converted from a binary representation of words selected,

where 1=selected, 0=unselected

3 = 11000

5 = 10100

6 = 01100

9 = 10010

10 = 01010

12 = 00110

17 = 10001

18 = 01001

20 = 00101

24 = 00011


So, if an answer is recorded as 3 -> that means the first two words of the list of five words were selected. In this dataset, an answer may also be -1 (subjected select 'don't know') or 0 (subject did not respond to question at all)

## Random questions

After the test there was an optional supplemental survey with some personality items and demographic questions.

This dataset only includes people who took the supplemental survey.

The following items were rated on a five point scale (1=Disagree, 5=Agree):

S1	I prefer to be barefoot.

S2	I avoid contacts with others.

S3	I had an imaginary friend as a child.

S4	I aposd rather not people pay attention to me.

S5	I would be interested in getting my fortune told.

S6	I am not what society wants me to be.

S7	I don't pack much luggage when I travel.

S8	I try my best to follow the rules.

S9	I did not work very hard in school.

S10	I don apost like to analyze literature.

S11	I sometimes feel like crying when I get angry.

S12	I am very unusual.

S13	I have been very interested in historical wars.

S14	I think ancient philosophy still is meaningful today.

S15	I have kept a personal journal.

S16	I have lots of my own theories.

S17	I could do an impressive amount of push ups.

S18	I put work first.

S19	I do not have a very expressive face.

S20	I do more than what apos;s expected of me.

S21	I sit on my legs.

S22	I am a perfectionist.

S23	I have studied how to win at gambling.

S24	I naturally emerge as a leader.

S25	I wish people were more spiritual.

S26	I always do the bare minimum I need to get by.

S27	I like to play devils advocate.

S28	I am not bothered by messy people.

S29	I am more artistic than scientific.

S30	I am not quite sure what I want.

## Biography questions

These questions were also asked:

age		How many years old are you?

gender		What is your gender? (1=Male,2=Female,3=Other)

engnat		Is English your native language? (1=Yes,2=No)

education	How much education have you completed? (1=Less than high school,2=High school,3=University degree,4=Graduate degree)

urban		What type of area did you live when you were a child? (1=Rural,2=Suburban,3=Urban)

