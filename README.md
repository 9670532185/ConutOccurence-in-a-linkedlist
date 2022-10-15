# ConutOccurence-in-a-linkedlist
public class SearchValueLL {
    public static class Node{
        int data;
        Node next;
        Node(int data)
        {
            this.data=data;
        }
    }
    public int CountValue(Node root,int val)
    {
        if(root==null)
        {
            return -1;

            
        }
        int count=0;
        
        while(root!=null)
       
        {
            if(root.data==val)
            {
                count++;
            }
            root=root.next;
        }
        return count;
    }
        // public boolean SearchValue(int value,Node root)
        // {
        //     if(root==null)
        //     {
        //         return false;
        //     }
        //     while(root!=null)
        //     {
        //         if(root.data==value)
        //         {
        //             return true;
        //         }
        //         root=root.next;
        //     }
        //     return false;
        // }
    // public boolean IsPresent(Node root,int x)
    // {
    //     if(root==null)
    //     {
    //         return false;
    //     }
    //     while(root!=null)
    //     {
    //         if(root.data==x)
    //         {
    //             return true;
    //         }
    //         root=root.next;
    //     }
    //     return false;
    // }
    public static void main(String[] args)
    {
        SearchValueLL obj=new  SearchValueLL();
        Node root=new Node(11);
        Node root1=new Node(12);
        Node root2=new Node(11);
        root.next=root1;
        root1.next=root2;
        System.out.println(obj.CountValue(root, 11));
        // System.out.println(obj.SearchValue(111,root));
        // System.out.println(obj.SearchValue(11,root));
      //  System.out.println(obj.IsPresent(root,1111111 ));
    }
    
}
