
package TwoPointers;

public class TwoSumSorted {

    public static void main(String[] args) {

        int[] a = {1, 2, 4, 6, 8, 9};
        int target = 12;

        int i = 0;
        int j = a.length - 1;

        while (i < j) {

            int sum = a[i] + a[j];

            if (sum == target) {
                System.out.println(i + " " + j);
                break;
            } else if (sum < target) {
                i++;
            } else {
                j--;
            }
        }
    }
}
