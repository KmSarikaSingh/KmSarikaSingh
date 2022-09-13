public static int findMax(int arr[], int n){
        int max1=1;
        int max2=0;
        
        for(int i=0;i<n;i++){
            int count=1;
            for(int j=0; j<n; j++){
                if(arr[i]==arr[j]){
                count+=1;
                }
            }
            
            if(max1<count){
                max1=count;
                max2=i;
            }
        }
        return max2;
    }
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int arr[]=new int[n];
        for(int i=0; i<n; i++){
            arr[i]=sc.nextInt();
        }
        Arrays.sort(arr);
        System.out.println(arr[findMax(arr,n)]);
