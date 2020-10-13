package com.tkravits;

import java.text.NumberFormat;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
    final byte Percent = 100;
    final byte Months_In_Year = 12;

	Scanner scanner = new Scanner(System.in);
	System.out.print("Principal: ");
	int principal = scanner.nextInt();

	System.out.print("Annual Interest Rate: ");
	double annual_interest = scanner.nextDouble();
	double monthInterestRate = annual_interest / Percent / Months_In_Year;

	System.out.print("Period (years): ");
	int years = scanner.nextByte();
	int time_period = years * Months_In_Year;

	double mortgage = principal * (monthInterestRate * Math.pow(1 + monthInterestRate, time_period)
			/ (Math.pow(1 + monthInterestRate, time_period) - 1));
	String mortgage_final = NumberFormat.getCurrencyInstance().format(mortgage);
	System.out.print("Mortgage Payment: " + mortgage_final);
    }
}
