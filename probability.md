# Probability

**probability:**<br>
(number of events) / (number of possible outcomes)<br>

**The ‘Or’ Rule:**<br>
P(B or R) = P(B) + P(R)<br>


**The ‘And’ Rule:**<br>
P(A and B) = P(A) x P(B)<br>

**Bayes' Theorem**<br>
P(A|B) =  P(A) * P(B|A) / P(B)<br>

Which tells us:<br>
    how often A happens given that B happens, written P(A|B),<br>
When we know:<br>
    how often B happens given that A happens, written P(B|A)<br>
 	 	and how likely A is on its own, written P(A)<br>
 	 	and how likely B is on its own, written P(B)<br>


# PROBABILITY PRACTICE PROBLEMS

1. On a six-sided die, each side has a number between 1 and 6. What is the probability of throwing a 3 or a 4? <br>

Ans: 2/6 = 1/3 <br>

2. Three coins are tossed up in the air, one at a time. What is the probability that two of them will land heads up and one will land tails up?

Ans: <br>
All choices  = HHH, THH, HTH, HHT, THT, TTH, HTT, TTT <br>
P(HHT) & P(HTH) & P(THH)  = 1/8 + 1/8 + 1/8  = 3/8 <br>

3. A two-digit number is chosen at random. What is the probability that the chosen number is a multiple of 7? <br>

Ans: <br>
Total Possibilitites = 10 to 99 = 09-10+1 = 90 <br>
Total Multiples of 7 netween 1 & 9 = 1 <br>
Total Multiples of 7 netween 1 & 100 = 14 <br>
Total multiples between 10 & 100 = 14-1 = 13 <br>
P(chosen number is multiple of 10) = 13/90 <br>

4. A bag contains 14 blue, 6 red, 12 green, and 8 purple buttons. 25 buttons are removed from the bag randomly. How many of the removed buttons were red if the chance of drawing a red button from the bag is now 1/3? <br>

Ans:  <br>
Total Buttons = 40 <br>
After 25 buttons are removed, # of buttons left = 15 <br>
No of reds left = x = 15/3 = 5    (1/3  = x/15)  <br>
Hence from total 6, no of removed buttons that were red are 1 <br>

5. There are 6 blue marbles, 3 red marbles, and 5 yellow marbles in a bag. What is the probability of selecting a blue or red marble on the first draw? <br>

Ans:  <br>
P(blue) = 6/14 <br>
P(red) = 3/14 <br>
P(blue or red) = 6/14 + 3/14 =9/14 <br>

6. Using a six-sided die, Carlin has rolled a six on each of 4 successive tosses. What is the probability of Carlin rolling a six on the next toss? <br>

Ans:  <br>
1/6   (The outcomes of previous rolls do not affect the outcomes of future rolls.)

7. A regular deck of cards has 52 cards. Assuming that you do not replace the card you had drawn before the next draw, what is the probability of drawing three aces in a row? <br>

Ans:  <br>
4/52 * 3/51 * 2/50 = 1/13 * 1/17 * 1/25 = 1/221 * 1/25 = 1/5525  <br> 

8. An MP3 player is set to play songs at random from the fifteen songs it contains in memory. Any song can be played at any time, even if it is repeated. There are 5 songs by B and A, 3 songs by B and B, 2 by B and C, and 5 by B and D. If the player has just played two songs in a row by B and D, what is the probability that the next song will also be by B and D? <br>

Ans:  <br>
Any song can be repeated in random
total songs = 15
total songs by B and D = 5
p(B and D) = 5/15 = 1/3


9. Referring again to the MP3 player described in Question 8, what is the probability that the next two songs will both be by B and B? <br>

Ans:  <br>
P (B and B) = 3/15
P (B and B & B and B) = 3/15 * 3/15 = 1/25


10. If a bag of balloons consists of 47 white balloons, 5 yellow balloons, and 10 black balloons, what is the approximate likelihood that a balloon chosen randomly from the bag will be black? <br>

Ans:  <br>
n(black) = 10
n(total) = 62
P(black) = 10/62  

11. In a lottery game, there are 2 winners for every 100 tickets sold on average. If a man buys 10 tickets, what is the probability that he is a winner? <br>

Ans:  <br>
First, simplify the winning rate. If there are 2 winners for every 100 tickets, there is 1 winner for every 50 tickets sold. This can be expressed as a probability of 1/50 or 0.02. In order to account for the (unlikely) scenarios of more than a single winning ticket, calculate the probability that none of the tickets win and then subtract that from 1. There is a probability of 49/50 that a given ticket will not win. For all ten to lose that would be (49/50)^(10) ≈ 0.817. Therefore, the probability that at least one ticket wins is 1 − 0.817 = 0.183 or about 18.3%



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


