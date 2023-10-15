
package CloudVandana;

	import java.util.Arrays;
	import java.util.Random;
   
	public class ArrayShuffle {

	    public static void main(String[] args) {
	         
	        int[] array = {1, 2, 3, 4, 5};
 
	        shuffleArray(array);
	         
	        System.out.println("Shuffled Array: " + Arrays.toString(array));
	    }

	    private static void shuffleArray(int[] array) {
	        int n = array.length;
	        Random random = new Random();

	        for (int i = n - 1; i > 0; i--) {
	            int randomIndex = random.nextInt(i + 1);

	             
	            int temp = array[i];
	            array[i] = array[randomIndex];
	            array[randomIndex] = temp;
	        }
	    }
	}
