# codigosimport java.util.Scanner;

public class Renda{
    public static void main(String[] args) {
        
    
    Scanner scanner = new Scanner(System.in);
    System.out.println("Salario do pai:");
    Double salarioPai = Scanner.nextdouble();
    System.out.println("Salario da esposa:");
    Double salarioMae = Scanner.nextdouble();
    System.out.println("numero de filhos:");
    int numeroFilho = Scanner.nextInt();

     Double rendaFamiliar = salarioPai + salarioMae;
     
     Double mediaRendaFamiliar = rendaFamiliar/2;

     Double numerodeFilho = (double)numeroFilho/2;

     Double maiorRendaFamiliar = Math.max(salarioPai, salarioMae);

     Double menosRendaFamiliar = Math.min(salarioPai, salarioMae);

     double maiorSalarioIndividual = Math.max(salarioPai, salarioMae);

     double menorSalarioIndividual = Math.min(salarioPai, salarioMae);

     Double[] salario = { salarioMae, salarioPai};
     
     int menorQue1500 = 0;
     for(double salario: salarios) {
        if(salario > 1500){
            menorQue1500++; 
        }
     }

     double percentual1500 = (Double) menorQue1500/ salarios.length* 100;
     System.out.printf("Média de renda familiar: R$ %.2f\n", mediaRendaFamiliar);
        System.out.printf("Média do número de filhos por família: %.2f\n",numerodeFilho);
        System.out.printf("Maior renda familiar: R$ %.2f\n", maiorRendaFamiliar);
        System.out.printf("Menor renda familiar: R$ %.2f\n", menosRendaFamiliar);
        System.out.printf("Maior salário individual: R$ %.2f\n", maiorSalarioIndividual);
        System.out.printf("Menor salário individual: R$ %.2f\n", menorSalarioIndividual);
        System.out.printf("Percentual de pessoas com salário menor que R$ 1500,00: %.2f%%\n",menorQue1500);
