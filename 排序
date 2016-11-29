package day13数组高级;

public class 排序 {
	public static void main(String[] args) {
		int[] arr = {23, 32, 2, 10, 3, 6, 9, 34, 1};
		数组输出(arr);
		System.out.println("--------------------");
		//冒泡排序(arr);
		选择排序(arr);
	}
	
	public static void 冒泡排序(int[] arr){
		for(int i = 0; i < arr.length; i++){
			for(int j = 0; j < arr.length-1-i; j++){
				if(arr[j] > arr[j+1]){
					int temp = arr[j];
					arr[j] = arr[j+1];
					arr[j+1] = temp;
				}
			}
			数组输出(arr);
		}
	}
	
	public static void 选择排序(int[] arr){
		for(int i = 0; i < arr.length; i++){
			for(int j = i+1; j < arr.length; j++){
				if(arr[i] > arr[j]){
					int temp = arr[i];
					arr[i] = arr[j];
					arr[j] = temp;
				}
			}
			数组输出(arr);
		}
	}
	
	
	public static void 数组输出(int[] arr){
		System.out.println("数组");
		System.out.print("[");
		for(int i = 0; i < arr.length; i++){
			if(i != arr.length-1){
				System.out.print(arr[i] + ", ");
			}else{
				System.out.print(arr[i] + "]");
			}
		}
		System.out.println();
	}
}
