arrays
======
public class Arrays {
	public static void main(String[] args) {
		int[] data = new int[3];
		
		for (int i = 0; i < data.length; i++) {
			data[i] = 10;

		}

		for (int i = 0, j=10; i < data.length; i++, j--) {
			data[i] = j;
		}

		sum(data);

	}

	public static int[] element(int[] a) {
		int x = 0;
		int y = 0;

		for (int i = 0 ; i < a.length; i++) {
			if (a[i] > x) {
				x = a[i];
			} else if


		}
	}
 
	public static int[] doubleIt(int[] a) {
		for (int i = 0; i < a.length; i++) {
			a[i] = a[i] * 2;
			printArray(a);

		}

		return a;
	}

	public static int[] sum(int[] a) {
		int sumEven = 0;
		int sumOdd = 0;
		int sumAll = 0;

		for (int i = 0; i < a.length; i++) {
			if (a[i] %2 == 0) {
				sumEven += a[i];
			} else {
				sumOdd += a[i];
			}


		}

		sumAll = sumEven + sumOdd;


		printArray(a);
		System.out.println("Sum of the Even: " + sumEven);
		System.out.println("Sum of the Odd: " + sumOdd);
		System.out.println("Sum of All: " + sumAll);

		return a;
	}



	public static void printArray(int[] a) {
		for (int i=0; i <a.length; i++) {
			System.out.print(a[i] + " ");
		}

	}
}
