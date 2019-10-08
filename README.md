# Singly_linkedlist

package elclipse;

public class Singlylinkedlist {

	public static class ListNode{
		private int data;
		private ListNode next;                           ////creating linked list

		public ListNode(int data) {
			this.data= data;
			this.next=null;
		}
	}
	public static void display(ListNode head) {
		if(head==null) {
			return;
		}
		ListNode current =head;
		while(current!=null) {
			System.out.print(current.data + " --> ");                 ////printing linked list
			current=current.next;
		}
		System.out.println("null");

	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		ListNode head= new ListNode(10);
		ListNode second= new ListNode(1);
		ListNode third= new ListNode(8);
		ListNode fourth= new ListNode(9);               

		head.next=second;
		second.next=third;
		third.next=fourth;

		Singlylinkedlist singly=new Singlylinkedlist();
		singly.display(head);                                                            
	}

}

