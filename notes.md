
# THIS IS JAVA IMPORTANT QUESTIONS 
* are objects iterable in java or not ?

In Java, an object is iterable if it implements the Iterable interface. For example:

ArrayList , LinkedList , HashSet , TreeSet , HashMap.keySet(), HashMap.values() (not the map itself)

`class Student 
{
    String name;
    int age;
}
`
this is not iterable directly , we need to implements iterable for the plain objects

`class MyContainer implements Iterable<String> {
    private String[] data = {"A", "B", "C"};

    public Iterator<String> iterator() {
        return Arrays.asList(data).iterator();
    }
}
`






# javascript 

* Tell me use of filter and map 


* map -- transform each element in the array

` const numbers = [1,2,3,4,5];
const squared = numbers.map((num)=>num*num) `

------in making todo application we can use map for updation 

* filter --return and array of elements which matches the condition 

`const nums = [1,2,3,4,5];
const even = nums.filter((num)=> num%2==0)`

-------in making todo application we can use filter for delete todos 



# BACKEND



# react 

* we can directly access the local storage until we are at the client side 

* Onclik me hmesha reference de skte hai function ni...but function jaisa dene liye callback Function ka use kr skte hai () => () 




# DBMS / SQL 

* Use on delete cascade 

If we are deleting something from the child table then it will be deleted automatically from the parent table

* Use of on delete set null

 If you are deleted from the parent table then the corresponding child table entry will be set as null

* Can foreign key have null value .
Yes the example is no delete set null


* Can we run select statements without using from ...

Yes , we can ,
SELECT 5+5 ;
SELECT  'hello world';

* When you remove from clause , my SQL treat it as selecting a single row with no columns, it allows you to evaluate expression directly 

* What is happening when we are using a group without any aggregation function

It is allowed but the values for non group columns are undefined or inconsistent
