jQuery CoreUISelect
===================

jQuery CoreUISelect is a cross browser easy to stylize select element with jQuery and CSS

## Available Features:

* Full customization
* Automatic calculations
* Keyboard support
* Powerful callback functions
* Compatible with mobile devices
* Support jScrollPane plugin for customize default scrollbar

See demo: http://shaggysmile.github.com/jQueryCoreUISelect/

## Default settings
    $('select').CoreUISelect();

## With jScrollPane plugin
    $('select').CoreUISelect({
        jScrollPane : {
           verticalDragMinHeight: 20,
           verticalDragMaxHeight: 20,
           showArrows : true
        }
     });
    
## Append to body

    $('select').CoreUISelect({
        appendToBody : true
    });

## Callback functions
Custom dropdown build in body

    $('select').CoreUISelect({
         onInit : addCoreUISelectListener,
         onOpen : addCoreUISelectListener,
         onClose : addCoreUISelectListener,
         onChange : addCoreUISelectListener,
         onDestroy : addCoreUISelectListener
     });
         
     function addCoreUISelectListener(select, event){
         console.log(el, event);
     } 
	 
## API
    $('select').CoreUISelect('update');
    $('select').CoreUISelect('destroy'); 	