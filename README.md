# Question-2
# Find the maximum consecutive 1's in an array of 0's and 1's. Example: a) 00110001001110 - Output :3 [Max num of consecutive 1's is 3] b) 1000010001 - Output :1 [Max num of consecutive 1's is 1]

public class Consecutive01 {
    
    static int[] a= {0,1,1,0,0,0,1,1,0,0,1,0};
    
    public static void main(String[] args) {
        int sum = 0;
        int max  = 0 ;
        for(int i = 0 ; i< a.length ; i++){
           if(a[i] == 0){
               sum = 0;
           } else {
               sum++;
               if(sum > max)
                   max = sum;
           }
        }
        
        System.out.println("Max consecutive 1s is: "+max);
    }
    
}
