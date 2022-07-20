import java.util.Scanner;

public class Rock_Paper_Scissors_Game {

    // 0 for Rock
    // 1 for paper
    // 2 for scissor
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double rand = Math.random() * 3;
        int comp_move = (int) Math.ceil(rand);
        System.out.println("Enter :->\n0 for Rock\n" +"1 for paper\n" +"2 for scissor\n");
        int user_move = sc.nextInt();
        if(user_move <= 2){
        if (comp_move == user_move) {
            System.out.println("Draw!!");
        } else if ((comp_move == 0 && user_move == 1) || (comp_move == 1 && user_move == 2)
                || (comp_move == 2 && user_move == 0)) {
            System.out.println("Congratulations!!, you defeated the computer");
        } else {
            System.out.println("You lost the game, the computer wins!!");
        }
        System.out.printf("\ncomputer move is %d\nYour move is %d ", comp_move, user_move);
        }
    else{
        System.out.println("Invalid move!!");
    }
    }
}
