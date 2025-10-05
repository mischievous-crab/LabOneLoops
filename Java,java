public class Main {
    public static void main(String[] args) {
        System.out.println(sumOdds(11));
        System.out.println(piApprox(100000));
        System.out.println(numTails(1000));
        System.out.println(countRolls(6, 100));
    }

    static int input;

    public static int sumOdds(int input_1) {
        input = input_1;
        int together = 0;

        for (int i = input_1; i >= 0; i--) {
            int inputCheck = input_1 - i;
            if ((inputCheck % 2) == 0) {
                together = together + 0;
            } else {
                together = together + inputCheck;
            }
        }

        return together;
    }

    public static double piApprox(double input) {
        int or = 0;
        double together = 0;
        double after = 0;

        for (int i = 0; i <= input; i++) {
            double inputCheck = 2 * i + 1;

            if ((or % 2) == 0) {
                after = 1 / inputCheck;
            } else {
                after = -1 / inputCheck;
            }

            together += after;
            or++;
        }

        return together * 4;
    }

    public static int numTails(int input) {
        int tails = 0;
        for (int i = 0; i <= input; i++) {
            double random = Math.random();
            if (random >= 0.5) {
                tails++;
            }
        }

        return tails;
    }

    public static int countRolls(int input1, int input2) {
        if (input1 <= 0 || input1 > 6 || input2 <= 0) {
            return -1;
        }

        int added = input1 * input2;
        int added2 = 0;
        int check = 0;

        while (added2 != added) {
            added2 = 0;

            for (int i = 0; i <= input2; i++) {
                double random = Math.random();
                if (random <= 1.0/6) {
                    added2 += 1;
                } else if (random <= 2.0/6) {
                    added2 += 2;
                } else if (random <= 3.0/6) {
                    added2 += 3;
                } else if (random <= 4.0/6) {
                    added2 += 4;
                } else if (random <= 5.0/6) {
                    added2 += 5;
                } else if (random <= 1) {
                    added2 += 6;
                }
                check++;
            }
        }

        return check;
    }
}
