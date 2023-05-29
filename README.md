# DraggableList
usage:
```
new Draggable(wrapper,view,holderClassName,cb);
```
wrapper:
```
The HTML Element of wrapper.
structure like this
<div id="wrapper">
  <div>1</div>
  <div>2</div>
  <div>3</div>
  ...
  <div>n</div>
</div>
```

view:  
The wrapper of list which can scroll. **default**: wrapper

holderClassName:  
The className of element in the listItem which can be hold to drag. **default**: 'holder'

cb: draggable => void  
The callback triggered after drop. **default**: a function to drop listItem to correct direction.


Draggable:  
&nbsp;&nbsp;&nbsp;&nbsp;wrapper: the same as 'wrapper' argument in constructor  
&nbsp;&nbsp;&nbsp;&nbsp;dragElem: the listItem be dragged  
&nbsp;&nbsp;&nbsp;&nbsp;firstIndex: the index of dragged element at first time  
&nbsp;&nbsp;&nbsp;&nbsp;currentIndex: the index of dropping position  
&nbsp;&nbsp;&nbsp;&nbsp;terminate(): revoke listen functions of Draggable  
&nbsp;&nbsp;&nbsp;&nbsp;...
