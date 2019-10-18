# COMP110 Worksheet 3: Flowcharts and pseudocode

![flowchart](https://github.com/Heathage/comp110-worksheet-3/blob/master/Fallout%204%20Minigame%20Flowchart.png)

```
LOAD Terminal Minigame
INPUT First Word from List of Words
SET First Guess True
WHILE First Word AND Second Word AND Third World not Correct or Guesses < 4
	IF First Guess True
		IF First Word NOT Correct
			CHECK First Word similarity to Correct Word		
CHECK List of Words for Same Similarity
			SET First Guess False AND Set Second Guess True
			PICK Second Word with Same Similarity As First Word
			ADD 1 to Guesses
		ELSE END LOOP
	ELSE IF Second Guess True
		IF Second Word NOT Correct
			CHECK Second Word similarity to Correct Word
			CHECK List of Words for Same Similarity
			SET Second Guess False AND Set Third Guess True
			IF Similarity Lower than First Word 
Pick Third Word with Similarity to First word AND Different to Second Word
				SET First Word as Sim Word
			ELSE IF Similarity Higher than First Word 
Pick Third Word with Similarity to Second word AND Different to First Word
				SET Second Word as Sim Word
			ELSE
				Pick Third Word with Similarity to First Word and Second Word
			Add 1 to Guesses
		ELSE END LOOP			
	ELSE IF Third Guess True
		IF Third Word NOT Correct
			CHECK Second Word similarity to Correct Word
			CHECK List of Words for Same Similarity
			SET Third Guess False AND Set Fourth Guess True
			IF Similarity Lower than Sim Word 
Pick Fourth Word with Similarity to Sim word AND Different to Third Word
			ELSE IF Similarity Higher than Sim Word 
Pick Fourth Word with Similarity to Third word AND Different to Sim Word
				SET Third Word as Sim Word
			ELSE
Pick Fourth Word with Similarity to First Word and Second Word and Third word
			Add 1 to Guesses
	ELSE END LOOP
	IF Fourth Word = Correct
		WIN
		UNLOCK TERMINAL
	ELSE
		ADD 1 to Guesses
END LOOP 

```
