# Functions
### Return Value
```cpp
int Homer() {
  Maggie=4;
  Return 7;
}

int main() {

  a=Homer();
    cout<<a<<endl; //Output: a = 7
    
    return 0;
 }
```
<table>
<tr>
<th>Pass-By-Value</th>
<th>Pass-By-Reference</th>
</tr>
<tr>
<td>
<pre>

A method of passing arguments to a
function where the value of the 
argument is passed. Changes made to 
the argument inside the function will 
not affect the original value.

</pre>
</td>
<td>
<pre>

a pass-by-reference refers to passing parameters to a function 
by using references.

It allows the ability to:
 Modify the value of the function arguments.
 Avoid making copies of a variable/object for performance reasons.

</pre>
</td>
</tr>
</table>

## Pass-By-Value



<table>
<tr>
<th>Pass-By-Value</th>
<th>Pass-By-Reference</th>
</tr>
<tr>
<td>

```cpp

void increment(int a) {
   a++; //a increases by 1
}

int main() {
   int x = 10;
   increment(x);
   cout << x; // Output: 10
}
```

</td>
<td>

```cpp
//a and b will be changed by the pass-by-reference
void swap_num(int &i, int &j) { //i = a, j = b
  int temp = i; //a = 100, temp = a, temp is now equal to 100
  i = j; //b = 200, a = b, a is now equal to 200
  j = temp; //temp = 100, b = temp, b is now equal to 100
}

int main() {
  int a = 100;
  int b = 200;

  swap_num(a, b);

  cout << "A is " << a << "\n"; //Output: A is 200
  cout << "B is " << b << "\n"; //Output: B is 100
}
```

</td>
</tr>
</table>



