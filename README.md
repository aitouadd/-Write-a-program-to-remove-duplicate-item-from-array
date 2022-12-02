# -Write-a-program-to-remove-duplicate-item-from-array


    //The indexOf() method returns the first index at which a given element can be found in the array, or -1 if it is not present.
         const arr = [1,2,3,4,1,2];
         const b=[];
              for(let i=0;i<arr.length;i++){
                 if(b.indexOf(arr[i]) == -1){
                     b.push(arr[i])
                 }
              }
             console.log("removed array value :",b)
       
    
   Output:   removed array value :  [1, 2, 3, 4]
               
             
             
             
*The filter() method creates a shallow copy of a portion of a given array,
filtered down to just the elements from the given array that pass the test implemented by the provided function.

*A shallow copy of an object is a copy whose properties share the same references (point to the same underlying values) 
as those of the source object from which the copy was made.







    const arr = [1,2,3,4,1,2];
    const b=[];
       arr.filter((dup)=>{
          if(b.indexOf(arr[dup]) == -1){
              b.push(arr[dup])
          }
       })
     console.log("removed array value :",b)
     
  Output:   removed array value :  [1, 2, 3, 4]
