import java.util.List;

public class Main {
    public static void main(String[] args) {
        System.out.println(sumCalibrationValues(Input.array));
    }
    
    public static int getIntegers(String input) {
        return Integer.parseInt(input.replaceAll("[^0-9]",""));
    }
    
    public static int getFirstInt(int number) {
        int first = 0;
        while (number > 0) {
            first = number % 10;
            number /= 10;
        }
        return first;
    }
    
    public static int getCalibrationValue(int number) {
        int last = number % 10;
        int first = getFirstInt(number);
        String concat = String.valueOf(first) + String.valueOf(last);
        return Integer.parseInt(concat);
    }
    
    public static int sumCalibrationValues(List<String> list) {
        int calibrationValue = 0;
        String next = "";
        int number = 0;
        int sum = 0;
        for (int i = 0; i < Input.array.size(); i++) {
            next = Input.array.get(i);
            number = getIntegers(next);
            calibrationValue = getCalibrationValue(number);
            sum += calibrationValue;
        }
        return sum;
    }
}
