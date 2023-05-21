import java.util.*;
public class lista {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner in =new Scanner (System.in);
		LinkedList <Integer> l1= new LinkedList <Integer> ();
		l1.add(1);
		l1.add(3);
		l1.add(5);
		l1.add(7);
		l1.add(9);
		
		System.out.println("Lista :"+l1);
		System.out.println("Elemento da agguingere:");
		int e= in.nextInt();
		int i=0;
		//one instruction
		while (i<l1.size() && e> l1.get(i)) 
			i++;
		l1.add(i,e);
		
		System.out.println("Lista :"+l1);
	
		
		System.out.println("Elemento da eliminare:");
		e= in.nextInt();
		i=0;
		while (i<l1.size() && e > l1.get(i)) 
			i++;
		
		if (i<l1.size() && e==l1.get(i)) {
			l1.remove(i);
			
		} else {
			System.out.println("Elemento inserito non esiste:");
		}
		System.out.println("Lista :"+l1);
	}

}


