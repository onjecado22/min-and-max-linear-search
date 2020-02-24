# min-and-max-linear-search

using namespace std; 
  
int search(int arr[], int n, int k) 
{ 
    int i; 
    for (i = 0; i < n; i++) 
        if (arr[i] == k) 
            return i; 
    return -1; 
} 
  
int main(void) 
{ 
    int arr[] = { 3, 4, 9, 12, 17 }; 
    int k = 10; 
    int n = sizeof(arr) / sizeof(arr[0]); 
    int result = search(arr, n, k); 
   (result == -1)? cout<<"Element is not present in array" 
                 : cout<<"Element is present at index " <<result; 
   return 0; 
