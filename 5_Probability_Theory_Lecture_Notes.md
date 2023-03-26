# Gambling and Uncertainty

Gambling deals with wagering on outcomes of events that are uncertain/unknown. Making predictions or "best guesses" based on information is known ex-ante (beforehand). First, we need some tools/terminology to describe groups of outcomes/numbers and their likelihoods of occuring.

## Standard Summary Statistics

- SET Notation: $A=\left\{a_1,\:a_2,\:a_3,\:...\:a_n\right\}$
    - e.g. $Student\:Age=\left\{19,\:19,\:20,\:24,\:19,\:21,\:18,\:20\right\}$
    - Can be order of non-ordered.
- *Sample Space*, S, List of possible values a set can take.
    - e.g. $S_A=\left\{18,\:19,\:20,\:21,\:24\right\}$

## Arithmetic

### Mean or Average:

Is a measure of the central tendency of a set of numbers

> $\overline{a}=\frac{1}{n}\sum _{i=1}^n\left(a_i\right)=\frac{19+19+20+24+19+21+18+20}{8}$
>> $\frac{160}{8}=20$

This may or may not be an element of set.

### Geometric Mean

> $\left(\prod_{i=1}^{n}x_{i}\right)^{\frac {1}{n}}={\sqrt[{n}]{x_{1}x_{2}\cdots x_{n}}}$
>> $={\sqrt[{8}]{(19)(19)(20)(24)(19)(21)(18)(20)}}$
>>> $=19.92$

### Median

"Middle value in an ordered set"
> $Student\:Age=\left\{18,\:19,\:19,\:19,\:20,\:20,\:21,\:24\right\}$
>> $= 19.5$

If $n$ is odd $med(a)=A\left(\frac{n+1}{2}\right)$  
If $n$ is even $med(a)=\frac{A\left(\frac{n}{2}\right)+A\left(\frac{n}{2}+1\right)}{2}$

> $\frac{A(H)+A(5)}{2}$
>> $\frac{19+20}{2}$

### Mode

Most common number in set. (Most likely to be drawn/sampled)

> $mode(A)=19$







When is $E[Winnings]>0$ ?  
When  
> $\$1.90+\frac{1}{t}\left(J*\frac{\$2\:million}{\$70\:million\:-\:J}+\$1\:million\frac{\$68\:million\:-\:J}{\$70\:million\:-\:J}\right) > 0$
>> $\frac{1}{\$1.90}\left(J*\frac{\$2\:million}{\$70\:million\:-\:J}+\$1\:million\frac{\$68\:million\:-\:J}{\$70\:million\:-\:J}\right)$  
>>> $t < \frac{5.9\:million}{\$1.90}$  
>>> $t < 3,105,263$  

If you know there was less than 3,105,263 million people playing than each ticket would have a positive expected winning given the 50 million jackpot.

# Probability of Craps

You roll 2 dice and sum their values.
- On your first roll, if you roll a 7 or 11: ${\color{red}Loss}$.
- On your first roll, if you roll a 2 or 3 or 12: ${\color{red}Loss}$.
- Otherwise if its not any of those sums, you establish the $point$ or $bench\:mark.$
- Then keep rolling either you make the point again (${\color{green}win\:double\:your\:bet}$) or you roll a 7 (${\color{red}lose}$), anything else and you keep rolling.

$E[Winnings]=\left( {\color{green}+} Bet \right)*Prob\left( 7 \cup 11 \right)$  
$E[Winnings]=\left( {\color{red}-} Bet \right)*Prob\left( 2 \cup 3 \cup 12 \right)$  
$E[Winnings]=\left( {\color{green}+} Bet \right)\sum_{i=4,5,6,8,9,10}^{}Prob\left(point_{i}|point_{i}\cup7\right)$  
$E[Winnings]=\left( {\color{red}-} Bet \right)\sum_{i=4,5,6,8,9,10}^{}Prob\left(7|point_{i}\cup7\right)$  