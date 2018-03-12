## 数组冒泡排序
```javascript
	 function bubbleSort(arr=[1,3,5,6,20,4,11,2,9,7]){
      	var len = arr.length;
    	for(var i=0;i<len;i++){
        	for(var j=1;j<len-i;j++){
            	if(arr[j-1]>arr[j]){
                	var temp = arr[j]
                    arr[j] = arr[j-1]
                  	arr[j-1] = temp
                }else{
                	continue
                }
            }
        }
        return arr;
    }
	console.log(bubbleSort());
	
	//[1, 2, 3, 4, 5, 6, 7, 9, 11, 20]
```