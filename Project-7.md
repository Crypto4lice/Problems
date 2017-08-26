# Project-7   #
## Data Structure - Tree ##

 >BST
 
    #define MAX_SIZE 100
	typedef struct node{
		int data;
		struct node *leftchild, *rightchild;
	}treenode;
	
	typedef treenode* treePtr;
	
	typedef struct _queue {
		treePtr arr[MAX_SIZE];
		int front;
		int rear;
	}queue;

	treePtr insert(treePtr* root, int key);
	treePtr delete(treePtr* root, int key);

	/* tree traversal */
	void Preorder(treePtr root);
	void Inorder(treePtr root);
	void Postorder(treePtr root);
	void Levelorder(treePtr root);

	/*       10
	        /   \
	       5     13
	     /   \      \
        4     7	     15
            /   \   /
           6     9 14

	*/




>위의 트리 구조를 가지는 BST를 구현하시오.
>Inorder의 경우 queue를 이용해서 구현하되 queue에 대한 ADT는 자유롭게 구성가능함