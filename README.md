# Algo
Explaining what i'v done in this Algo code:

1- Determine the length of the sentence (The number of the character).
2- Counting the number of words in the sentence (if the words are separated by space).
3- Counting the number of vowels in the sentence.

---------------------------------------------------------------------------------------------------------------------------------



VAR
    ph: STRING[50];
    i: INTEGER:=0;
    cptChar, cptW, cptV:INTEGER;

BEGIN

# Initializing a counter for vowels,Words and characters
    cptChar:= 0;
    cptV:= 0;
    cptW:= 1;

    Write("Give me the sentence: ");
    Read(ph);
    ph.toLower();

    WHILE (ph[i] <> '.') DO
        cptChar:= cptChar +1;
        
# Define a function to check for space
        IF (ph[i]= ' ') THEN
            cptW:= cptW +1; 
        END_IF
        
# Define a function to check for vowels
        IF (ph[i] in ['e','i','o','a','u']) THEN
            cptV:= cptV +1; 
        END_IF

        i:= i+1;

        
# Printing the results
    END_WHILE
    Write("Length of the sentence:", cptChat);
    Write("Number of words in the sentence:", cptW)
    Write("Number of vowels in the sentence:", cptV)
END
