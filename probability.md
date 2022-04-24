# Probability

**probability:**
(number of events) / (number of possible outcomes)

**The ‘Or’ Rule:**
P(B or R) = P(B) + P(R)


**The ‘And’ Rule:**
P(A and B) = P(A) x P(B)

**Bayes' Theorem**
P(A|B) =  P(A) * P(B|A) / P(B)

Which tells us:	 	
    how often A happens given that B happens, written P(A|B),
When we know:	 	
    how often B happens given that A happens, written P(B|A)
 	 	and how likely A is on its own, written P(A)
 	 	and how likely B is on its own, written P(B)


# PROBABILITY PRACTICE PROBLEMS

1. On a six-sided die, each side has a number between 1 and 6. What is the probability of throwing a 3 or a 4?

Ans: 2/6 = 1/3

2. Three coins are tossed up in the air, one at a time. What is the probability that two of them will land heads up and one will land tails up?

Ans: 
All choices  = HHH, THH, HTH, HHT, THT, TTH, HTT, TTT
P(HHT) & P(HTH) & P(THH)  = 1/8 + 1/8 + 1/8  = 3/8

3. A two-digit number is chosen at random. What is the probability that the chosen number is a multiple of 7?

Ans: 
Total Possibilitites = 10 to 99 = 09-10+1 = 90
Total Multiples of 7 netween 1 & 9 = 1
Total Multiples of 7 netween 1 & 100 = 14
Total multiples between 10 & 100 = 14-1 = 13
P(chosen number is multiple of 10) = 13/90

4. A bag contains 14 blue, 6 red, 12 green, and 8 purple buttons. 25 buttons are removed from the bag randomly. How many of the removed buttons were red if the chance of drawing a red button from the bag is now 1/3?

Ans: 
Total Buttons = 40
After 25 buttons are removed, # of buttons left = 15
No of reds left = x = 15/3 = 5    (1/3  = x/15) 
Hence from total 6, no of removed buttons that were red are 1

5. There are 6 blue marbles, 3 red marbles, and 5 yellow marbles in a bag. What is the probability of selecting a blue or red marble on the first draw?

Ans: 
P(blue) = 6/14
P(red) = 3/14
P(blue or red) = 6/14 + 3/14 =9/14

6. Using a six-sided die, Carlin has rolled a six on each of 4 successive tosses. What is the probability of Carlin rolling a six on the next toss?

Ans: 

7. A regular deck of cards has 52 cards. Assuming that you do not replace the card you had drawn before the next draw, what is the probability of drawing three aces in a row?

Ans: 

8. An MP3 player is set to play songs at random from the fifteen songs it contains in memory. Any song can be played at any time, even if it is repeated. There are 5 songs by Band A, 3 songs by Band B, 2 by Band C, and 5 by Band D. If the player has just played two songs in a row by Band D, what is the probability that the next song will also be by Band D?

Ans: 

9. Referring again to the MP3 player described in Question 8, what is the probability that the next two songs will both be by Band B?

Ans: 

10. If a bag of balloons consists of 47 white balloons, 5 yellow balloons, and 10 black balloons, what is the approximate likelihood that a balloon chosen randomly from the bag will be black?

Ans: 


 # Example

&nbsp;

**Imagine you have a jar of 500 coins. 1 out of 500 is a coin with two heads and all the others have a tail and a head. You take a random coin from the jar and flip it 8 times. You observe heads 8 consecutive time. Are the chances that you took the coin with two heads higher than having drawn a regular coin with a head and a tail?**
 
The main tool is Bayes Theorem. 

Define A the event of tossing the chosen coin and having heads 8 times, `B_1` and `B_2` the events of choosing the special and fair coins respectivly. We compute the odd of choosing the special coin over the fair one given the event A.
 - `P(B_1|A) : P(B_2 |A)`

If this odd is greater than 1, then the answer is yes. Otherwise, no.

By Bayes theorem (some manipulations),
- `P(B_1|A) : P(B_2 |A) = (P(A|B_1) P(B_1)) : (P(A|B_2) P (B_2)) ` 
- `= ( P(A|B_1)/ P(A| B_2) ) * (P(B_1) / P(B_2) (*)`
 
 The second ratio is the odd of choosing the special coin over the fair one. It equals `1/499`.
 
 The first ratio is `1/(1/2)^8 = 256`.

So the odd of choosing the special coin over the fair one given the event A is `256/499` which <1. Hence there is a lower chance that we took the special coin than the fair one.

Extra comments:
 - From the solution, if there were 9 consecutive heads, then the odd would be 512/499 and hence the answer would be `yes`.
 - The formula (*), in general, has [the form ](https://en.wikipedia.org/wiki/Likelihood_ratios_in_diagnostic_testing#Estimation_of_pre-_and_post-test_probability)
 
      `post-odd = likelihood ratio of the event A * pre-odd`
 - Another solution is to compute directly `P(B_1|A)` by using Bayes and total probability theorems,
 
   ``` 
   P(B_1|A) = P(A|B_1) P(B_1) / P(A) = P(A|B_1) P(B_1) / (P(A|B_1) P(B_1) + P(A|B_2) P(B_2))
   = 1 * (1/500) / (1/500 + (1/2)^8 * (499/500)) 
   ```
   and see that it is `<1`
 - The problem contains several implicit assumptions. For example: 
   - A with one head and tail is called **fair** under the assumption that both sides have equal chance to land in each toss.
   - We assume that each toss results in a head or a tail face but no other scenarios (like standing)
<br/>


