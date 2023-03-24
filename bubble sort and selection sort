#include <iostream>
#include <vector>

using namespace std;

void quickSort(vector<int>& arr, int left, int right) {
    if (left >= right) return;

    int pivot = arr[(left + right) / 2];
    int i = left, j = right;

    while (i <= j) {
        while (arr[i] < pivot) i++;
        while (arr[j] > pivot) j--;
        if (i <= j) {
            swap(arr[i], arr[j]);
            i++;
            j--;
        }
    }

    quickSort(arr, left, j);
    quickSort(arr, i, right);
}
void bubble_sort(int a[],int n){
    //In the above implementation,
    // a boolean flag swapped is used to keep track
    // of whether any swap occurred
    // during a pass through the array
    // . If no swap occurred during a pass,
    // it means that the array is already sorted
    // and the outer loop can be terminated early.
    bool flag;
    for (int i = 0; i < n-1; i++) {
        flag= false;
        for (int j = 0; j < n-i-1; j++) {
            if (a[j]>a[j+1]){
                swap(a[j],a[j+1]);
                flag= true;
            }
        }
        if (!flag)break;
    }
}
int main() {
    vector<int> arr = { 5, 2, 7, 1, 8, 3, 6, 4 };
    quickSort(arr, 0, arr.size() - 1);

    for (int num : arr) {
        cout << num << " ";
    }
    cout << endl;

    return 0;
}
