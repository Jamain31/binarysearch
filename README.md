# binarysearch
Java program that uses a binary search algorithm looking for the numbers 17 and 45 from an array.

This is a Java program that uses a binary search algorithm looking for the numbers 17 and 45 from an array.

package mainPAckage;
//Binary Search Algorithm
//Jamain Hughes
//Carl Marquez
//CPT307: Data Structures and Algorithms
//09/26/2022
public class searchProgram {

	public static void binarySearch(int arr[], int first, int last, int key) {
		
		int mid = (first + last)/2;
		
		while( first <= last ) {
			if ( arr[mid] < key) {
				first = mid + 1;
			}else if ( arr[mid] == key ){
				System.out.println(" Element " + key + " is found at index: " + mid);
				
				break;
			}else {
				last = mid - 1;
			}
			mid = (first + last)/2;
		}
		
		if ( first > last ) {
			System.out.println(" Element " + key + " is not found! ");
		}
		
		
		
	}
	
	public static void main(String args[]) {
		int arr[] = {5,10,15,20,25,30,35,40,45,50,55,60,65,70};
		int key = 17;
		int key2 = 45;
		int last=arr.length-1;
		binarySearch(arr,0,last,key);
		binarySearch(arr,0,last,key2);
		System.out.println(" Binary Search Algorithm");
		System.out.println(" Jamain Hughes ");
		System.out.println(" Carl Marquez ");
		System.out.println(" CPT307: Data Structures and Algorithms ");
		System.out.println(" 09/26/2022 ");
		
		
		
	}
	 

		
		
	
	

}

![binarysearch1](https://user-images.githubusercontent.com/108758588/195983241-179b970e-f7d3-4b84-bf0c-22d4f55387dd.png)
![binarysearch2](https://user-images.githubusercontent.com/108758588/195983249-d17310b0-afab-41df-ba53-8dad182909d9.png)
