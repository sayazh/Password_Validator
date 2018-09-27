# Password_Validator
based_on_simple_ways
package Day_15_StringManipulation;

import java.util.Scanner;

public class passValid {
	public static void main(String[] args) {
		Scanner scan = new Scanner(System.in);
		System.out.println("     Password requirements: ");
		System.out.println(" - Be a minimum of eight (8) characters in length");
		System.out.println(" - Contain at least one upper case letter (A-Z)");
		System.out.println(" - Contain at least one lower case letter (a-z)");
		System.out.println(" - Contain at least one digit (0-1-2-3-4-5-6-7-8-9");
		System.out.println(" -Contain at least one special character (`~!@#$%^&*()[]:;?/)");
		System.out.println("     ENTER PLEASE NEW PASSWORD ");
		
		String password = scan.nextLine();
		if (password.length() >= 8) {
			if (password.indexOf("A") > -1 || password.indexOf("B") > -1 || password.indexOf("C") > -1
					|| password.indexOf("D") > -1 || password.indexOf("E") > -1 || password.indexOf("F") > -1
					|| password.indexOf("G") > -1 || password.indexOf("H") > -1 || password.indexOf("I") > -1
					|| password.indexOf("J") > -1 || password.indexOf("K") > -1 || password.indexOf("L") > -1
					|| password.indexOf("M") > -1 || password.indexOf("Q") > -1 || password.indexOf("R") > -1
					|| password.indexOf("S") > -1 || password.indexOf("T") > -1 || password.indexOf("U") > -1
					|| password.indexOf("V") > -1 || password.indexOf("W") > -1 || password.indexOf("X") > -1
					|| password.indexOf("Y") > -1 || password.indexOf("Z") > -1) {
				if (password.indexOf("a") > -1 || password.indexOf("b") > -1 || password.indexOf("c") > -1
						|| password.indexOf("d") > -1 || password.indexOf("e") > -1 || password.indexOf("f") > -1
						|| password.indexOf("g") > -1 || password.indexOf("h") > -1 || password.indexOf("i") > -1
						|| password.indexOf("j") > -1 || password.indexOf("k") > -1 || password.indexOf("l") > -1
						|| password.indexOf("m") > -1 || password.indexOf("n") > -1 || password.indexOf("o") > -1
						|| password.indexOf("p") > -1 || password.indexOf("q") > -1 || password.indexOf("r") > -1
						|| password.indexOf("s") > -1 || password.indexOf("t") > -1 || password.indexOf("u") > -1
						|| password.indexOf("v") > -1 || password.indexOf("u") > -1 || password.indexOf("w") > -1
						|| password.indexOf("x") > -1 || password.indexOf("y") > -1 || password.indexOf("z") > -1) {
					if (password.indexOf("`") > -1 || password.indexOf("~") > -1 || password.indexOf("!") > -1
							|| password.indexOf("@") > -1 || password.indexOf("#") > -1 || password.indexOf("$") > -1
							|| password.indexOf("%") > -1 || password.indexOf("^") > -1 || password.indexOf("&") > -1
							|| password.indexOf("*") > -1 || password.indexOf("(") > -1 || password.indexOf(")") > -1 || 
							password.indexOf("[")>-1 || password.indexOf("]")>-1 || password.indexOf("|")>-1 || 
							password.indexOf("<")>-1 || password.indexOf(">")>-1 || password.indexOf(",")>-1 || password.indexOf(".")>-1 ||
							password.indexOf("?")>-1 || password.indexOf(":")>-1 || password.indexOf(";")>-1 || password.indexOf("/")>-1 ) {
						if (password.contains("0") || password.contains("1") || password.contains("2") || password.contains("3")
								|| password.contains("4") || password.contains("5") || password.contains("6")
								|| password.contains("7") || password.contains("8") || password.contains("9")) {
							System.out.println("CONGRATULATIONS!!! Your password is accepted");
						} else {
							System.out.println("Password should have at least one digit number");
						}
					} else {
						System.out.println("Password should contain at least 1 of these special characters: "+
					
							"`~!@#$%^&*()[]:;?/" );
					}
				} else {
					System.out.println("Password should contain at least 1 lowercase letter");
				}
			} else {
				System.out.println("Password should contain at least 1 uppercase letter");
			}
		} else {
			System.out.println("Password should contain minimum 8 characters");

		}  scan.close();


		}
	} 
