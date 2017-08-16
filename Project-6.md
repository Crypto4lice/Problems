#  Problem 6 # Data structure #
----------


>Linked list


    typedef struct node {
		int data;
		struct node* link;
	}listnode;

	typedef listnode* nodePtr;

	void insert();
	void delete();
	nodePtr search();
    

>Stack
	
	
    #define MAX_SIZE 100
	typedef struct _stack {
		int arr[MAX_SIZE];
		int top;
	};
	
	struct _stack stack;

	void isempty();
	void isfull();
	void push();
	int pop();
	int peak();


>Queue

    Update soon
