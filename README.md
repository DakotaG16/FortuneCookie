# FortuneCookie
import java.io.File;
import java.util.Scanner;

public class Program {

	public static void main(String[] args) {
		File f = new File("Fortune.txt");
		
		try {
			Scanner sc = new Scanner(f);
			while(sc.hasNextLine()) { 
				String fortune = sc.nextLine();
			if(fortune.endsWith(".")){
				System.out.println(fortune);
			}
			else {
					System.out.println(fortune +".");
			}
			}
		 
			
		}
		catch(Exception e) {
			System.out.println("bad");
		}

	}

}
