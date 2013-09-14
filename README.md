Angularjs-DragAndDrop
=====================

And Angularjs module to implement HTML5 Dran And Drop behavior.

DEMO
----
http://plnkr.co/edit/Y3C6QUPgAuT3ZkA3bDyB?p=preview


READ ABOUT HTML5 DRag&DROP
--------------------------

For better understanding, read at:
https://developer.mozilla.org/en-US/docs/DragDrop/Drag_and_Drop

DRAGGABLE :: directive
----------------------

Draggable attribute must contain the model which will be passed to the droppable.
e.g <div data-draggable="myModel">
where myModel is in the parent controller scope.

It supports the following attributes as well:

dropOn:         drop-on:        array|string  This defines on which droppables it can be dropped only.
dragImageAttr:  drag-image:     array|string  Where array format allows to pass x and y offsets  e.g [images/dragIcon.png, 0, 10]
effectAllowed:  effect-allowed: string        This can be one between copy, move, link, copyLink, copyMove, all, none, uninitialized
onDragStart:    on-drag-start:  function
onDrag:         on-drag:        function
onDragEnd:      on-drag-end:    function


DROPPABLE
---------

dropId:         on-drop-id:        string        This identifies uniquely this droppable, in such a way that draggables containing it in array or string forma, will be able to drop in it.
onDragEnter:    on-drag-enter:     function
onDragOver:     on-drag-over:      function
onDrop:         on-drop:           function
