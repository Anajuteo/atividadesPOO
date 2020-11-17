import java.util.Scanner;

public class exercicio1 {
	
	public static void main(String[] args) {
		
		Scanner entrada = new Scanner(System.in);
		
		float peso;
		double altura;
		double pesoH;
		double pesoM;
		char sexo;
		
		
		System.out.println("Informe o sexo (M/F): ");
		sexo = entrada.nextLine().charAt(0);
		
		System.out.println("Informe a altura: ");
		altura = entrada.nextDouble();
		
		System.out.println("Informe o peso: ");
		peso = entrada.nextFloat();
		
		pesoH = (peso*altura) - 58;
		pesoM = (peso*altura) - 44.7f;
		
		
		if (sexo == 'M')
		{
			System.out.printf("Seu peso ideal é: ", pesoH);
		}
		else if (sexo == 'F')
		{
			System.out.printf("Seu peso ideal é: ", pesoM);
		}
		
	 }
}
