public static void check(int ar[],int m,int n,int arr[]){
        
        for(int i=0;i<n;i++){
            int count=0;
            for(int j=0;j<m;j++){
                if(arr[i]+ar[j]==0){
                    System.out.println(arr[i]);
                }
            }
            
        }
    }
	public static void main(String[] args) {
		Scanner sc=new Scanner(System.in);
		int n=sc.nextInt();
		int arr[]=new int[n];
		for(int i=0;i<n;i++){
		    arr[i]=sc.nextInt();
		}
		int m=sc.nextInt();
		int ar[]=new int[m];
		for(int i=0;i<m;i++){
		    ar[i]=sc.nextInt();
		}
		
		    check(ar,m,n,arr);
		
	}
