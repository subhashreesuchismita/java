package order;

public class customer {
private int customerld;
private String customerName;
private String customerAddress;
private order order;
public customer(int customerld, String customerName, String customerAddress, order order) {
	super();
	this.customerld = customerld;
	this.customerName = customerName;
	this.customerAddress = customerAddress;
	this.order = order;
}
@Override
public String toString() {
	return "customer [customerld=" + customerld + ", customerName=" + customerName + ", customerAddress="
			+ customerAddress + ", order=" + order + "]";
}

}

public class order {
	private int orderld;
	private String itemName;
	private double itemPrice;
	public order(int orderld, String itemName, double itemPrice) {
		super();
		this.orderld = orderld;
		this.itemName = itemName;
		this.itemPrice = itemPrice;
	}
	@Override
	public String toString() {
		return "order [orderld=" + orderld + ", itemName=" + itemName + ", itemPrice=" + itemPrice + "]";
	}
	

}
package order;

public class mainprogram {
public static void main(String[]args) {
	order ob1=new order(123,"Burger",565);
	customer ob2= new customer(232,"Lucky","cuttack",ob1);
	System.out.println(ob2);
}
}
