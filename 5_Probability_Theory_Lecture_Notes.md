# Section Title

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