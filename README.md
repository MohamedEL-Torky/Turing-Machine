# Turing-Machine
Java program that determine if the transations you've entered will accepted or rejected.

HOW TO USE:
-----------
Enter how many states your language have excluding the accept and reject state.
Enter the number of the alphabets your language accept including Blank.
-----------
Transations
-----------
Enter the transation state as fllow:
1-Enter what this state name, state alphabet then hit enter.
2-Enter what this state will do when it reads this alphabet in the tape eg.(move to state, update, move right or left on the tape).
3-Continue repeating step 1 and 2 till the loop breaks.
----
Tape
----
Enter the tape alphabets.
Enter the head postion, it can be any number assuming the tape has infinte blanks after the last alphabet you've entered.
------
Output
------
You will see each move and choosen transation the program will take and at the end it will reject or accpet.
Note the if you've an error in your transations the program will loop forever,
because it will not reach the accept nor the reject state.
---------------------------------------------------------------------------------------------------------------------------------
Logic behind the code:
----------------------
1-By getting the number of states and the alphabets we can get how many transtions will be in the language by multiplying the
state number with the alphabets number, since turing machine states are deterministic.

2-Getting the language transations the first part as key and the second as a value usinbg Hashes, 
and assuming your langugae state start counting from q1.

3-The program will enter in infinite loop till it accept or reject the tape.

4-Inside the loop the tape will being updated with each update it encounter in the transations and will not updated if it was the
same symbol on the first part of the transation.

5-Getting the current state the tape on and the current alphabet the head pointing on the tape by combining them togither the
program concatenate them togither and make them as a key and get it's value on the hash map we get
(move to state, update, move right or left on the tape) so our current state now = move to state,
our tape current alphabet will be update with update from the retrived value more R or L will move the tape right or left.
---------------------------------------------------------------------------------------------------------------------------------
Note:
-----
If you're confused with how to enter the transations look at the transation.txt uploaded in this repository.
---------------------------------------------------------------------------------------------------------------------------------
For further inquires contact me on mohamedtarekeltorky@gmail.com or leave a comment.
