

!/bin/bash 

# This script is rock scissor paper game

#


echo "Rock, Paper, Scissors"


#This variables to keep track of win, loose, tie


w=0

l=0

t=0



while true

do

#the main game loop

while true

do

        echo "$w Wins, $l Losses, $t Ties";

        read -p "Enter (r)ock (p)aper (s)cissors, q to quit " player_move #input of player


        if [[ "$player_move" == "q" ]];

        then

                exit


#tried to exit loop but did'nt work, used 2 while loops without break           

#       elif [[ "$player_move" == "r" || "$player_move" == "p" || "$player_move" == "s" ]];

#       then

                #done

        else

                echo "Type one of r, p, s, or q."

        fi

        #done


# Display what the player choose

#

if [[ "$player_move" ==  "r" ]];

then

        echo "ROCK versus..."

elif [[ "$player_move" == "p" ]];

[7/21 6:29 PM] Ibrokhim Khodjimukhamedov

then

        echo "PAPER versus..."

elif [[ "$player_move" == "s" ]];

then

        echo "SCISSORS versus..."

fi


#Display what the computer chose:


random_number=$(expr 1 + $RANDOM % 3 );   #Generates random number between 1, 2, and 3

if [[ $random_number = 1 ]];              #Converts random number into string ROCK=1 PAPER=2 

then                                      #SCISSORS=3   

        comp_move="r"

        echo "ROCK"

elif [[ $random_number = 2 ]];

then

        comp_move="p"

        echo "PAPER"

elif [[ $random_number = 3 ]];

then

        comp_move="s"

        echo "SCISSORS"

fi


#Display and record the win/loss/tie:


if [[ "$comp_move" == "$player_move" ]]; #Compares variables of player and machine

then

        echo "Tie";

        ((t+=1));                        #Records results 

elif [[ "$comp_move" == "s" && "$player_move" == "r" ]];

then

        echo "You win!";

        ((w+=1));

elif [[ "$player_move" == "p" && "$comp_move" == "r" ]];

then

        echo "You win!";

        ((w+=1));

elif [[ "$player_move" == "s" && "$comp_move" == "p" ]];

then


echo "You win!";

        ((w+=1));

elif [[ "$player_move" == "r" && "$comp_move" == "p" ]];

then

        echo "You lose!";

        ((l+=1));

elif [[ "$player_move" == "p" && "$comp_move" == "s" ]];

then

        echo "You lose!";

        ((l+=1));

elif [[ "$player_move" == "s" && "$comp_move" == "r" ]];

then

        echo "You lose!";

        ((l+=1));

fi

done   #second while loop for continious input of player


done   #First loop for continious game
