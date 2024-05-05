## Two-pointer approach

```
public int fn(int[] arr){
    int left = 0;
    int right = arr.length -1;
    int ans = 0;
    while(left < right){
        //do some logic
        if(condition){
            left++;
        }else{
            right--;
        }
    }
    return ans;
}
```
