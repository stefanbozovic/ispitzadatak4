U produžetku teksta je dat kod klase sa metodom koja bi trebalo da, na ekranu, ispisuje strelicu od znakova
0. Ideja je da strelica bude visine šest redova, širine 5 znakova i okrenuta “na dole”, tako da bi konačan ispis
na ekranu trebalo da bude:

		0

		0
   
		0
   
	0   0	0

	   000
 
		0
Dati kod se kompajlira, ali ne radi to šta treba. Napraviti javnu klasu IspisivacStrelice2 u paketu
ispravka_koda, prekucati u nju kod koji je dat i, uz minimalne izmene ga ispraviti tako da funkcioniše
kako treba. Napraviti test klasu i, koristeći njenu main metodu, pozvati metodu ispisiStrelicu2() i proveriti
njen rad.

package ispravka_koda;

	public class IspisivacStrelice2 {
	
		public static void ispisiStrelicu2() {
		
			for (int i=1; i<7; i++) {
			
				for(int j=1; j<6; j++)
				
					if (j==1 || i-j==2 || i+j==9)
					
						System.out.print('0');
						
					else
					
						System.out.print(' ');
						
			}
			
	}
	
}