# mith DropDown
A simple reusable drop down component for mithril js framework.
This component is intended to create reusable drop down lists as a component in [mithril js.](http://mithril.js.org/)
A list as an array is passed in to the object as it is beig instantiated and the drop down is created with the array.
###[Live on jsFiddle](https://jsfiddle.net/pharzan/ar20pL37/1/)
```javascript
var list=['Banana','Apple','Orange','Kiwi'];
var myList=new MythDropDown(list);
```
Then the component can be used in any mithril view:
```javascript
var main={
	view:function(){
    	return m.component(myList);
    }
}
```
And the created view can be placed in the DOM:

```javascript
var main={
	view:function(){
    	return m.component(myList);
    }
}
```
For easier usage the component has the following functions which can be accessed directly:
* update() //updated the drop down with a new list
* sort() //sort the drop down
* delete() //remove the selected item
* getSelected() // returns the selected items name and index.

Any of the above functions can be accessed in the examples below:
```javascript
 var L1=['Yellow','Black','Orange','Brown','Red'];
  	 myList.update(L1);
     myList.sort();
     myList.delete();
     console.log(myList.selected.name);
     console.log(myList.selected.index);
```

## Links

* [GitHub](https://github.com/pharzan/mithDropDown) Repository	
 * [Mith Drop Down](http://pharzan.github.io/mithDropDown) page
 * [jsFiddle](https://jsfiddle.net/pharzan/ar20pL37/1/) live on jsFiddle
 * [mithril.js](mithril.js.org)
 
