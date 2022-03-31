# Sum-of-odd-length-in-subarray

 int arr[]={1,2,3,4,5};
      int finalsum=0;
      
      for(int i=0; i<arr.length; i++)
      {
        for(int j=i; j<arr.length; j++)
        { 
          
          String str= "";
          int sum=0;
          
          if((j-i+1)%2==1) // %2==0 for even subarrays value REMOVE this if condion for print all value
          {
             for(int k=i; k<=j; k++)
             {
                str = str+arr[k];
                sum =sum+arr[k];
             }
             finalsum=finalsum+sum;
             System.out.println(str+"-->"+sum);
          }
        
        }
      }
      System.out.println(finalsum);
