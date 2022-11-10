# DERS
Koşullarla Beden Kitlesi Hesaplama
package ders;

import java.util.Scanner;

public class dersK {

	public static void main(String[] args) {
		
		
		Scanner klavye = new Scanner(System.in);
		
		System.out.print("Kilonuz : ");
		int kilo = klavye.nextInt();
		
		System.out.print("Boy (Örnek : 1,80)");
		
		double boy = klavye.nextDouble();
		
		double bki = (kilo / (boy * boy));
		
		if ( bki < 18.5) {
			System.out.println("Zayıf");
		}
		else if ( bki >= 18.5 && bki < 25) {
			System.out.println("Normal");
			
		}
		else if (bki >=25 && bki < 30) {
			System.out.println("Fazla kilolu");
		}
		else {
			System.out.println("Obez");
		}
		
		
		
		
	}
	

}
