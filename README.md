# Binary-Search
Binary Search is a searching algorithm for finding an element's position in a sorted array.In this approach, the element is always searched in the middle of a portion of an array.<br>
Binary search can be implemented only on a sorted list of items. If the elements are not sorted already, we need to sort them first.<br>
<br>
# Binary Search Working:-<br>
1.The array in which searching is to be performed is:<br>
<br>
![image](https://user-images.githubusercontent.com/125802204/234284364-cb6929c3-0e90-4315-9a3d-a7a455de057c.png)
<br>
Let x = 4 be the element to be searched.<br>
2.Set two pointers low and high at the lowest and the highest positions respectively.<br>
<br>
![image](https://user-images.githubusercontent.com/125802204/234284569-37fa0cdc-8611-4156-9423-0748e557c673.png)
<br>
3.Find the middle element mid of the array ie. arr[(low + high)/2] = 6.<br>
<br>
![image](https://user-images.githubusercontent.com/125802204/234284711-db8b1d18-326d-4bf1-9596-7e4ad8288f5f.png)
<br>
4.If x == mid, then return mid.Else, compare the element to be searched with m.<br>
<br>
5.If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.<br>
<br>
6.Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.<br>
<br>
![image](https://user-images.githubusercontent.com/125802204/234284981-bb384e69-ad14-4c3c-aa86-be41cc940f03.png)
<br>
7.Repeat steps 3 to 6 until low meets high.<br>
<br>
![image](https://user-images.githubusercontent.com/125802204/234285130-d3a5e8ae-9445-4588-9729-e9687145ee06.png)
<br>
8.x = 4 is found.<br>
<br>
![image](https://user-images.githubusercontent.com/125802204/234285263-06de432f-9906-487c-8915-aa971738ec9b.png)
<br>
# Binary Search Algorithm:- <br>
<br>
binarySearch(arr, x, low, high)<br>
    if low > high<br>
        return False <br>
    else<br>
        mid = (low + high) / 2 <br>
        if x == arr[mid]<br>
            return mid<br>
        else if x > arr[mid]        // x is on the right side<br>
            return binarySearch(arr, x, mid + 1, high)<br>
        else                               // x is on the left side<br>
            return binarySearch(arr, x, low, mid - 1)<br>
            <br>
            <br>
<b><ins> Time Complexities</b></ins><br>
<br>
<ol><b>Best case complexity:</b></ol> O(1)<br>
<br>
<ol><b>Average case complexity:</b></ol> O(log n)<br>
<br>
<ol><b>Worst case complexity:</b></ol> O(log n)<br>
<br>
<b><ins>Space Complexity</b></ins><br>
<br>
The space complexity of the binary search is O(1).<br>
<br>
# Applications:- <br>
<br>
1. In libraries of Java, .Net, C++ STL<br>
2.While debugging, the binary search is used to pinpoint the place where the error happens.<br>
<br>
<br>
<b><ins>Output</b></ins>
<br>
<img width="936" alt="Binary Search" src="https://user-images.githubusercontent.com/125802204/234288554-e4a57e70-e025-473b-82bf-1c80b4147770.png">




