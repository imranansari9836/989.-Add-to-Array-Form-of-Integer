class Solution {
    public List<Integer> addToArrayForm(int[] num, int k) {
        List<Integer>list=new ArrayList<>();
        for(int i=num.length-1;i>=0||k>0;i--)
        {
            int sum=k;//34
            if(i>=0)//3>=0
            {
                sum=sum+num[i];//34+0
            }
            int b=sum%10;//34%10=4
            list.add(0,b);//4
            k=sum/10;//3
        }
        return list;// [1,2,3,4]
    }
}
