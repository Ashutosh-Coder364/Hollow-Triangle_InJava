public class Pattern_Hollow_Triangle {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            for (int j = 1; j <= i; j++) {
               if(i > 2 && j == 2 && i < 5 || i == 4 && j == 3) {
                    System.out.print("  ");
                }
                else{
                    System.out.print("$ ");
                }
            }

            System.out.println("");
        }
    }
}
