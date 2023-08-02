# firstGame
This is "Scissors Paper Rock" game. This game was made by 30/7/2023 by me. Hope the next time, i look this description again, i can make it better.
function getComputerChoice(){
    let pick=["Rock","Scissors","Paper"];
    return pick[Math.floor(Math.random()*pick.length)];
}
    let playerSelction= prompt("Choose one",);
function playRound(playerSelection, computerSelection) {
    if(computerSelection ==="Rock" && playerSelction === "Scissors"){
        alert ("You lose! Rock beats Scissors");
    } else if ( computerSelection === "Rock" && playerSelction === "Paper"){
        alert ("You win! Paper beats Rock");
    } else if ( computerSelection === "Paper" && playerSelction === "Scissors"){
        alert("Your win! Scissors beats Paper");
    } else if (computerSelection === "Paper" && playerSelction === "Rock"){
        alert("You lose! Paper beats Rock");
    } else if (computerSelection === "Scissors" && playerSelction === "Paper"){
        alert ("You lose! Scissors beats Paper");
    } else if (computerSelection === "Scissors" && playerSelction === "Rock"){
        alert("You win! Rock beats Scissors");
    } else if ( computerSelection === "Scissors" && playerSelction === "Scissors" || computerSelection === "Rock" && playerSelction === "Rock" ||computerSelection === "Paper" && playerSelction === "Paper"){ 
        alert("That's a tie, babieeeeee. Let's play again!");
    } else {
    alert ("Sorry, I can't figure out what you choose X_X");
}
}

console.log(playRound(playerSelection, computerSelection));
