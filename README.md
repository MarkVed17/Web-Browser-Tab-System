# Web-Browser-Tab-System

## Created a **web browser tab system** type functioning in C using _Stack_ data structure.
_Browser Tab Functioning_ could be one of the application of _Stack_ as a Data Structure. We add tabs similar to adding books on a stack. A stack is a container of objects that are inserted and removed according to the last-in first-out **(LIFO)** principle. In the pushdown stacks only two operations are allowed: push the item into the stack, and pop the item out of the stack. A stack is a limited access data structure - elements can be added and removed from the stack only at the top. Push adds an item to the top of the stack, pop removes the item from the top. A helpful analogy is to think of a stack of books; you can remove only the top book, also you can add a new book on the top. A browser has several functions, few of which are Adding a Tab, Adding an Incognito Tab, View History, Add to Bookmarks, View Bookmarks, Recent Tabs. Each can be converted to a proper function. First create a Struct stack comprising of members as 2-D char arrays - site, history, bookmark & their respective tops – int top, top1, top2. Define the 2-D char arrays size [MAX1] & [MAX2] initially as 100 each, can exceed depending on the user. Now we can store a maximum of 100 websites on our browser i.e. user can add upto 100 tabs. Let’s frame the functions in our browser with respect to a Stack. In our case the elements or data type that we will be handling is going to be a char array i.e. a String. User will be provided with a Menu to interact with the Browser. 
Menu consists of :

-  _Adding a Tab_, 
-  _Adding an Incognito Tab_,
- _Back_, 
- _Add to Bookmarks_, 
- _Recent Tabs_, 
- _View Bookmarks_, 
- _View History_, 
- _Exit_. 

The numbers adjoining the functions are the choices menu will offer the user. A tab will be added on entering 1, an incognito type of tab will be added on entering 2,…,Exit the program on entering 8. 

---

## 1. Add a Tab :
Basically a push function to add an element onto 
the Stack. Return type void. It will ask the user “Enter Search
Text” & the will push or add the text i.e. String onto the site 
& history stack. 
void push(stack *s, int ch) ;
top of the Stacks will be incremented appropriately on 
adding a tab. 

---

## 2. Add an Incognito Tab: 
Similar as adding a tab, but, as an 
incognito tab works, the searched text won’t be added to 
the history but will only be present onto Recent tabs(Private 
Search). This is done by adding an if statement in the 
function void push(stack *s, int ch) ;
If(ch! =2) // It’s not an incognito tab. 
Then procedure will be as usual. 

---

## 3. Back: 
Similar to pop function, the top is then pointing to the 
previously entered String. This function only works on site
stack thus not changing the history stack. So, a Search Text once 
entered is forever present in the history but if user chooses back
 or pops then site stack will be void of that pointing String. 

---

## 4. Add to Bookmarks: 
This function allows the user to add any 
searched text to the bookmarks. On choosing 4, a list of 
searched texts will be displayed on Screen from which the 
user can bookmark any text. This function adds that String 
onto the Bookmark stack. 

---

## 5. Recent Tabs : 
It displays a list of all the searched texts that 
are entered by the user. It also includes search via incognito 
tabs. Point to note, the popped Strings won’t be there on 
the Recent Tabs. Recent Tabs are modified after each 
push/pop function. 

---

## 6. View Bookmarks: 
It displays a list of all search texts added 
on to the bookmark stack. Incognito Tabs can’t be 
bookmarked and hence won’t be displayed as they aren’t 
present on the history stack. 

---

## 7. View History: 
It displays an entire list of search texts 
including all the pushed and popped Strings. It keeps a track 
of all the entered search texts. 

---

## 8. Exit : 
On choosing this, the program execution is immediately terminated.

---

_Open to all the discrete ideas which can progress this project._
