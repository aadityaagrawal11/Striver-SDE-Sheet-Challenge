class Queue {
    int* arr;
    int q_front;    //data memeber issue over front
    int rear;
    int size;
public:
    Queue() {
        // Implement the Constructor
        //not getting size => give size default
        size = 100001;
        arr = new int[size];
        q_front = 0;
        rear = 0;    //starting set
    }

    /*----------------- Public Functions of Queue -----------------*/

    bool isEmpty() {
        // Implement the isEmpty() function
        if(q_front==rear){
            return true;
        }
        else{
            return false;
        }
    }

    void enqueue(int data) {
        // Implement the enqueue() function
        if(rear == size){
            cout<<"Q full";
        }
        else{
            arr[rear] = data;
            rear++;
        }
    }

    int dequeue() {
        // Implement the dequeue() function
        if(rear==q_front){
            return -1;
        }
        else{
            int ans = arr[q_front];
            arr[q_front] = -1;
            q_front++;
            if(q_front==rear){
                q_front = 0;
                rear = 0;
            }
            return ans;
        }
    }

    int front() {
        // Implement the front() function
        if(q_front == rear){
            //empty
            return -1;
        }
        else{
            return arr[q_front];
        }
    }
};
