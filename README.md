# test1
class parentclass{
	int a;
	parentclass(int x){
		a=x;
	}
}
class childclass extends parentclass{
	int b;
	childclass(int x,int y) {
		
		super(x);
		b=y;
		
	}
	void show() {
		System.out.println("value of a: "+a+"\n valueof b:"+b);
	}

	
}
public class orderOfExecution {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		System.out.println("order of constructor execution");
		
		childclass obj=new childclass(55,65);
		obj.show();
	}

}
