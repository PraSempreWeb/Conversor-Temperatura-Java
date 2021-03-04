# Fala Dev´s  :vulcan_salute:
 

<h1 align="center"> 
	 Conversor de Temperatura Java   :man_technologist:
<h1 align="center">  
	
	
	
	
[![Linkedin Badge](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white&link=https://www.w3schools.com/java/default.asp)](https://www.w3schools.com/java/default.asp) [![Linkedin Badge](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&link=https://www.linkedin.com/in/prasempreweb/)](https://www.linkedin.com/in/prasempreweb/)
	

### Escreva um programa que, com base em uma temperatura em graus celsius, a converta e exiba em Kelvin (K), Réaumur (Re), Rankine (Ra) e Fahrenheit (F), seguindo as fórmulas: F = C * 1.8 + 32; K = C + 273.15; Re = C * 0.8; Ra = C * 1.8 + 32 + 459.67.  

**Fahrenheit (F)** - Unidade de medida de temperatura em que os pontos de congelação e de ebulição da água são, respetivamente, de 32 °C e 212 °C.  
**Kelvin(K)** - O kelvin é a escala fundamental da temperatura termodinâmica, e seus instrumentos de medidas (termômetros) estão, normalmente, graduados com os pontos de fusão do gelo a 273 K e o ponto de ebulição da água a 373 K, considerando as condições normais de pressão.  
**Rankine (Ra)** - A escala Rankine (símbolo R, Ra) é uma escala de temperatura absoluta assim chamada em homenagem ao engenheiro e físico escocês William John Macquorn Rankine, que a propôs em 1859. Assim como a escala absoluta Kelvin, o 0 Ra é o zero absoluto, porém a variação do Rankine é definida como sendo igual a um grau Fahrenheit. Assim, a variação de um Ra equivale à variação de um °F. Então a temperatura de -459,67 °F é exatamente igual a 0 Ra.  
**Réaumur (Re)**- A escala Réaumur (símbolo: °Ré, °Re, °R) é uma escala de temperatura proposta em 1730 pelo físico e inventor francês René-Antoine Ferchault de Réaumur, cujos pontos fixos são o ponto de congelamento da água (0°Ré) e seu ponto de ebulição (80°Ré). Assim, a unidade desta escala, o grau Réaumur, vale 5/4 de 1 grau Celsius e a escala tem o mesmo zero que a escala Celsius.   
**Celsius (°C)** - O grau Celsius ou centígrado é uma unidade que se utiliza para expressar a grandeza física temperatura e representa-se por oC. ... Esta unidade de temperatura deve o seu nome ao astrónomo sueco Anders Celsius. Este ficou conhecido por propor em 1742 o uso da escala Celsius.   



```
import java.util.Locale;
import java.util.Scanner;

public class ConversorTemperatura {

	public static void main(String[] args) {
		// TODO Auto-generated method stub		
		Scanner sc = new Scanner(System.in);
		Locale.setDefault(Locale.US);  
    
   //Declaração de Variaveis
		double C, K, F, Re, Ra;  
    
		//Entrada de dados  
		System.out.print("Digite a temperatura em graus Celcius: ");
		C = sc.nextDouble();	
    
		F = C * 1.8 + 32;
		K = C + 273.15;
		Re = C * 0.8;
		Ra = C * 1.8 + 32 + 459.67;  
    
		System.out.println();  
		System.out.printf("A temperatura em graus Celcius " + C + " convertida em Fahrenheit (F) = %.2f%n", F);
		System.out.printf("A temperatura em graus Celcius " + C + " convertida em Kelvin (K) = %.2f%n", K);
		System.out.printf("A temperatura em graus Celcius " + C + " convertida em Réaumur (Re) = %.2f%n", Re);
		System.out.printf("A temperatura em graus Celcius " + C + " convertida em Rankine (Ra) = %.2f%n", Ra);
		sc.close();	
	}
}
```
