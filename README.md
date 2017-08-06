# SelectionSort
java选择排序
//冒泡排序

public class BubbleSort {
   public static void main(String[] args) {
	   //定义一个数组并进行快速赋值
	   int[] num = new int[]{6,5,4,3,2,1};
	   for(int i:num){
		   System.out.print(i+" ");
	   }
	   System.out.println("\n");
	   //升序排列
	   //两两比较
	   int temp;
	   int count=0;
	   for(int j=0;j<num.length-1;j++){
		   //如果将每次循环的结果打印出来我们可以看到
		   //事实上外层循环只需要num.length-1次就行了
		   for(int i=0;i<num.length-j-1;i++){
			   //这里第一轮将最大值移动到了最后，
			   //所以第二轮只需要比较前面五个数就行了
			   //所以内层循环就是num.length-1
			   //一定要注意我们后面比较的是i和i+1
			   //所以这里的i的终止条件为num.length-1
			   //防止溢出
			   if(num[i]>num[i+1]){
				   temp=num[i];
				   num[i]=num[i+1];
				   num[i+1]=temp;
			   }
		   }
		   count++;
		   System.out.print("第"+count+"次：");
		for(int i:num){
			System.out.print(i+" ");
			
		}
		System.out.println("\n");
	   }
	  
} 
	   
}
