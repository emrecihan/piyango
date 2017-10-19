package hafta6_1;
import java.util.Scanner;

public class algo6_1 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		//verileri yarat
		int input1, input2, sistem1, sistem2; 
		
		//rastgele iki sayý yarat
		sistem1=(int) (Math.random()*10);
		sistem2=(int) (Math.random()*10);
		System.out.println("sayýlar= "+sistem1+"ve" +sistem2);
		
		//kullanýcýdan iki sayý girmesini iste
		System.out.println("lütfen 0 ile 9 arasýnda sayý giriniz=");
		Scanner input=new Scanner(System.in);
		input1= input.nextInt();
		input2= input.nextInt();
		
		
		//karþýlaþtýrmalarý yap ve gerekli mesajý göster
		if(input1==sistem1 && input2==sistem2)
			System.out.println("$1.000 kazandýnýz");
		else if(input1==sistem2 && input2==sistem1)
			System.out.println("$3.000 kazandýnýz");
		else if(input1==sistem1 || input1==sistem2 || input2==sistem1 || input2==sistem2)
			System.out.println("$10.000");
		else
			System.out.println("bir dahaki sefere");
			

	}
	
	

}
