## Two-pointers: one input, opposite ends

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

## Two-pointers: two inputs, exhaust both

```
public int fn(int[] arr1, int[] arr2){
    int i =0, j=0, ans = 0;
    while(i < arr.length  && j < arr2.length){
        //do some logic
        if(condition){
            i++;
        }else{
            j++;
        }
    }
    while(i<arr1.length){
        //do logic
        i++;
    }
    while(j<arr2.length){
        //do logic
        j++;
    }
    return ans;
}
```

## Sliding window

```
public int fn(int[] arr){
    int left = 0, ans = 0, curr = 0;
    //do logic here to add arr[right]  to curr
    while(WINDOW_CONDITION_BROKEN){
        //remove arr[left] from curr
        left++;
    }
    //update ans
    return ans;
}
```

## Build a prefix sum

```
public int[] fn(int[] arr){
    int[] prefix = new int[arr.length];
    prefix[0] = arr[0];

    for(int i=1;i<arr.length;i++){
        prefix[i] = prefix[i-1] + arr[i];
    }
    return prefix;
}
```

## Linked list: Fast and slow pointer

```
public int fn(ListNode head){
    ListNode slow = head;
    ListNode fast = head;
    int ans = 0;

    while(fast!=null && fast.next!=null){
        //do logic
        slow = slow.next;
        fast = fast.next.next;
    }
    return ans;
}
```

## Reversing a Linked list

```
public ListNodefn(ListNode head){
    ListNode curr = head;
    ListNode prev = null;

    while(curr!=null){
        ListNode nextNode = curr.next;
        curr.next = prev;
        prev = curr;
        curr = nextNode;
    }
    return prev;
}
```
