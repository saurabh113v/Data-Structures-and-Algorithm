// Java program to merge two sorted linked lists
// using array
import java.util.*;

class Node {
    int data;
    Node next;

    Node(int x)
    {
        data = x;
        next = null;
    }
}

class GfG {

    // Function to merge two sorted linked lists
    static Node sortedMerge(Node head1,
                                       Node head2) {
        ArrayList<Integer> arr = new ArrayList<>();

        // Pushing the values of the first linked list
        while (head1 != null) {
            arr.add(head1.data);
            head1 = head1.next;
        }

        // Pushing the values of the second linked list
        while (head2 != null) {
            arr.add(head2.data);
            head2 = head2.next;
        }

        // Sorting the list
        Collections.sort(arr);

        // Creating a new list with sorted values
        Node dummy = new Node(-1);
        Node curr = dummy;

        for (int i = 0; i < arr.size(); i++) {
            curr.next = new Node(arr.get(i));
            curr = curr.next;
        }

        return dummy.next;
    }

    static void printList(Node curr) {
        while (curr != null) {
            System.out.print(curr.data);
            if (curr.next != null) {
                System.out.print(" ");
            }
            curr = curr.next;
        }
        System.out.println();
    }

    public static void main(String[] args) {

        // First linked list: 5 -> 10 -> 15
        Node head1 = new Node(5);
        head1.next = new Node(10);
        head1.next.next = new Node(15);

        // Second linked list: 2 -> 3 -> 20
        Node head2 = new Node(2);
        head2.next = new Node(3);
        head2.next.next = new Node(20);

        Node res = sortedMerge(head1, head2);
        printList(res);
    }
}
