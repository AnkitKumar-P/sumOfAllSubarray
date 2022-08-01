# sumOfAllSubarray

// sumOfAllSubarray

#include <iostream>
using namespace std;

// sumOfAllSubarray
void sumOfAllSubarray(int arr[], int size)
{
    int count = 0;
    for (int i = 0; i < size; i++)
    {
        int sum = 0;
        for (int j = i; j < size; j++)
        {
            sum = sum + arr[j];
            cout << sum << endl;
            count++;
        }
    }
    cout << "Total subarray : " << count;
}

int main()
{
    int arr[] = {1, 2, 0, 7, 2};
    sumOfAllSubarray(arr, 5);

    return 0;
}
