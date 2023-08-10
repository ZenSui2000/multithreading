# multithreading

1. Multithreading is defined as the ability of a processor to execute multiple threads concurrently.Multithreading makes multitasking possible when it breaks programs into smaller, executable threads.Threading Module

2. Threading module is used for creating, controlling and managing threads in python.

a. Returns the number of thread objects that are active
b.Returns the number of thread objects in the caller's thread control.
c.The enumerate function is a built-in function that allows you to iterate through a sequence and keep track of the index of each element.

3. a.The run() method invokes the callable object passed to the object's constructor as the target argument, if any, with positional and keyword arguments taken from the args and kwargs arguments, respectively.
b.The start() method is an inbuilt method of the Thread class of the threading module, it is used to start a thread's activity.
c.Join in Python is an in-built method used to join an iterable's elements, separated by a string separator, which is specified by you.
d.The isAlive() method checks whether a thread is still executing.

4. import threading

def print_cube(num):

	print("Cube: {}" .format(num * num * num))

def print_square(num):

	print("Square: {}" .format(num * num))

if __name__ =="__main__":

	t1 = threading.Thread(target=print_square, args=(20,))
	t2 = threading.Thread(target=print_cube, args=(20,))

	t1.start()
	t2.start()


	t1.join()
	t2.join()

	print("Done!")

 5. 1. Advantages are : performance, responsiveness, and resource utilization

2. Disadvanatges are : 
Difficulty of writing code. 
Difficulty of debugging. 
Difficulty of managing concurrency. 
Difficulty of testing. 
Difficulty of porting existing code.

6. Race conditions are when two threads use the same variable at a given time.

Deadlock exists when two threads seek one lock simultaneously.
