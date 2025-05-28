import java.util.Arrays;
public class Main {
    public static void main(String[] args) {
        int [] a={5,1,6,3,2,4};
        int n=a.length;
        int[] res={a[0],a[1]};
        int ms=a[0]+a[1];
        for(int i=0;i<=n-2;i++){
            for(int j=i+1;j<=n-1;j++){
                if(a[i]+a[j]>ms){
                    ms=a[i]+a[j];
                    res[0]=a[i];
                    res[1]=a[j];
                }
            }
        }
        System.out.println(Arrays.toString(res));
    }
}
