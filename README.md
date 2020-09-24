# Test
Test git
import java.util.Map;

public class Week4 {
    /**
     * Return the bigger number.
     * @param a the first num
     * @param b the second num
     * @return max of $a and $b
     */
    public static int max2Int(int a, int b) {
        if(a > b) {
            return a;
        }
        return b;
    }

    /**
     * Return the smallest number of the array.
     * @param arr input array
     * @return min of array $arr
     */
    public static int minArray(int[] arr) {
        int min = arr[0];
        for (int i = 0; i < arr.length; i++) {
            if(min > arr[i]) {
                min = arr[i];
            }
        }
        return min;
    }

    /**
     * Return the BMI.
     * @param weight: in kg
     * @param height: in m
     * @return BMI index
     */
    public static String calculateBMI(double weight, double height) {
        double BMI = weight / height / height;
        double Round_Off = Math.round(BMI*10.0)/10.0;
        if (Round_Off < 18.5){
            return "Thiếu cân";
        }
        if (Round_Off >= 18.5 && Round_Off <= 22.9){
            return "Bình thường";
        }
        if (Round_Off <= 24.9 && Round_Off >= 23){
            return "Thừa cân";
        }
        if (Round_Off >= 25){
            return "Béo phì";
        }
        return null;
    }
}
