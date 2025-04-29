# cs1010s-tutorial-6-strings-and-vectors-solved
**TO GET THIS SOLUTION VISIT:** [CS1010S Tutorial 6-Strings and Vectors Solved](https://www.ankitcodinghub.com/product/cs1010s-tutorial-6-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;115100&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS1010S Tutorial 6-Strings and Vectors Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
1. string s and vector s are passed by value copy, in and out of functions. This is different from C-strings and arrays, which are passed by pointers.

Consider the following functions:

char * capitalize(char *s) { for (int i = 0; s[i]; i++) if (‘a’ &lt;= s[i] and s[i] &lt;= ‘z’) s[i] -= 32;

return s;

}

string capitalize(string s) { for (int i = 0; i &lt; s.size(); i++) if (‘a’ &lt;= s[i] and s[i] &lt;= ‘z’) s[i] -= 32;

return s; }

Note: in C++ it is ok to have functions of the same name, provided the input signature is different. The compiler will match the type of the arguments to determine which function to call.

(a) What is the output when the following lines of code are executed? Try to figure it out before running the program.

char cstring[20] = “Hello World!”; char *new_cstr; string stdstring = “Hello World!”, new_stdstr;

new_cstr = capitalize(cstring); new_stdstr = capitalize(stdstring);

printf(“C-string: %s “, cstring); printf(“New C-string: %s “, new_cstr); cout &lt;&lt; “std::string: ” &lt;&lt; stdstring &lt;&lt; endl; cout &lt;&lt; “New std::string: ” &lt;&lt; new_stdstr &lt;&lt; endl;

(b) What happens when the signature of the second function is changed to

i. string capitalize(string &amp;s) ii. string &amp;capitalize(string &amp;s)

1

(c) Come up with some code to demonstrate the same effect with arrays and vectors.

However, it is not entirely necessary to depend on these functions to insert and erase elements from a string/vector. We can always write our own insert and erase function to suit our needs as such: vector&lt;int&gt; my_vector = {0, 1, 2, 3, 4, 5}; insert(my_vector, 2, 10); // inserts into index 2 erase(my_vector, 5); // removes element at index 5

for (int i = 0; i &lt; my_vector.size(); i++) cout &lt;&lt; my_vector[i] &lt;&lt; ” “;

This will result in an output of 0 1 10 2 3 5 .

Provide an implementation for the functions insert and erase using only the member functions .push_back , .pop_back and .size .

4. The function void mutate takes in a vector of int, and sets each element to the sum of its neighbours, with the ends wrapping around.

For example, the vector 0, 1, 2, 3, 4, 5 will mutate to 1+5, 0+2, 1+3, 2+4, 3+5, 4+0 .

Provide an implementation for the function void mutate .
