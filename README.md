HumanPlayerTest
===============

import java.util.Scanner;

public class HumanPlayerTest{//used to implement human player but was difficult in calling classes
	
	public static int[] main(String[] args) {

		Board gameBoard = new Board();
		Play play = new Play();
		HumanPlayer HumanPlay = new HumanPlayer();


		
	    
		gameBoard.displayBoard();
		HumanPlayer.Enter();// wasn't sure how to properly call this, reason it wont work
		play.setPlay(point[0],point[1],point[2],point[3]);
		System.out.println("Expected: X "+point[0]+"-"+point[1]+" "+point[2]+"-"+point[3]);
		gameBoard.doPlay(Board.X_PLAYER, play);
		gameBoard.displayBoard();
		HumanPlayer.Enter();
		System.out.println("Expected: O "+point[0]+"-"+point[1]+" "+point[2]+"-"+point[3]);
		gameBoard.doPlay(Board.O_PLAYER, play);
		gameBoard.displayBoard();

	}

}

