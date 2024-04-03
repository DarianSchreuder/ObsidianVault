# Searching
2023-05-24 | 00:12
{Subject}:[[CMPG 211]]
{Section}:[[Searching]]
{Tags}: #Programming #Java 
{Related}:

--- 
```run-java
public static binarySearch(int[] array, int num)
{
	int first = 0;
	int last = array.length - 1;
	int midpoint = (first + last)/2;
	boolean found = false;
	while(first <= last && !found)
	{
		if(array[midpoint] == num)
			found = true;
		else if(item < array[midpoint])
			last = midpoint - 1;
		else
			first = midpoint + 1;
	}
	if (found == true)
		return midpoint;
	else
		return -1;
}

public static void main(string[] args)
{
	int arr[] = {17, 20, 26, 31, 44, 54, 55, 65, 77, 93};
	System.out.printf("The value 50 is at index %d\n",binarySearch(arr,50));
	System.out.printf("The value 44 is at index %d\n",binarySearch(arr,44));
}
```

--- 
{Efundi Lecture Notes}: [Searching]()