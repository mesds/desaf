# desaf
desafio de programação 


1- <!-- java -->
public class Escada {

    public static void main(String args[]) {
        
        System.out.print("* * *\n"
        +                "    *\n"
        +                "    * * *\n"
        +                "        *\n"
        +                "        *\n");
    }
}**



2- 
public static boolean validaSenha(String senha) {

        String regex = "^(?=.*[0-9])"
                + "(?=.*[a-z])(?=.*[A-Z])"
                + "(?=.*[!@#$%^&*()-+])"
                + "(?=\\S+$).{6}$";

        Pattern p = Pattern.compile(regex);


        if (senha == null) {
            return false;
        }



        Matcher m = p.matcher(senha);

        return m.matches();
    }

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        System.out.println("Nome");
        String nome = scanner.next();
        System.out.println("Senha");
        String senha = scanner.next();



        System.out.println(validaSenha(senha));
    }


}





