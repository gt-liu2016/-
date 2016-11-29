package day13数组高级;

import java.util.Scanner;

public class 查找 {
	public static void main(String[] args) {
		// 无序的数组只能使用基本查找，不能使用二分查找
		int[] arr1 = { 23, 32, 2, 10, 3, 6, 9, 34, 1 };
		数组输出(arr1);
		Scanner sc = new Scanner(System.in);
		int num1 = sc.nextInt();
		int xx = 基本查找(arr1, num1);
		System.out.println("num: " + num1 + "\nindex: " + xx);
		// 二分查找、折半查找对有序的数组进行快速查找
		int[] arr2 = { 1, 2, 3, 6, 9, 10, 23, 32, 34 };
		数组输出(arr2);
		int num2 = sc.nextInt();
		int yy = 二分查找(arr2, num2);
		System.out.println("num: " + num2 + "\nindex: " + yy);
		sc.close();
		//Arrays.binarySearch(arr2, num2);
	}
	
	//二分查找
	public static int 二分查找(int[] arr, int num){
		int max = arr.length-1;
		int min = 0;
		int mid = (max+min)>>>1;
		while (arr[min] != num) {
			if (arr[mid] > num) {
				max = mid - 1;
			} else {
				min = mid + 1;
			}
			if (min > max) {
				return -1;
			}
			mid = (max + min) >>> 1;
		}
		return mid;
	}
	
	//基本查找，从头到尾遍历，直到查找到相应的数字停止
	public static int 基本查找(int[] arr, int num){
		int i = 0;
		for(; i < arr.length; i++){
			if(arr[i] == num){
				break;
			}else if(arr[i] != num && i == arr.length-1){
				return -1;
			}
		}
		return i;
	}
	
	// 数组输出
	public static void 数组输出(int[] arr) {
		System.out.println("数组");
		System.out.print("[");
		for (int i = 0; i < arr.length; i++) {
			if (i != arr.length - 1) {
				System.out.print(arr[i] + ", ");
			} else {
				System.out.print(arr[i] + "]");
				System.out.println();
			}
		}
	}
}
