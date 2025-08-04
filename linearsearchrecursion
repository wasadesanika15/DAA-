#include <stdio.h>

void read1(int a[], int n);
int linearSearch(int a[], int key, int index, int n);

int main() {
    int n, key, index;
    
    printf("Enter n value : ");
    scanf("%d", &n);
    
    int a[n];
    
    printf("Enter %d elements : ", n);
    read1(a, n);
    
    printf("Enter a key element : ");
    scanf("%d", &key);
    
    index = linearSearch(a, key, 0, n);
    
    if (index == -1) {
        printf("The key element %d is not found\n", key);
    } else {
        printf("The key element %d is found at position : %d\n", key, index);
    }
    
    return 0;
}

// Function to read elements into array
void read1(int a[], int n) {
    for (int i = 0; i < n; i++) {
        scanf("%d", &a[i]);
    }
}

// Recursive linear search function
int linearSearch(int a[], int key, int index, int n) {
    if (index >= n) {
        return -1;
    }
    if (a[index] == key) {
        return index;
    }
    return linearSearch(a, key, index + 1, n);
}
