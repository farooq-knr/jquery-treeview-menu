# .treeviewMenu() #

## Overview ##
```
.treeviewMenu(options)
.treeviewMenu(method, arg, ...)
```

### Sample ###
```
:
<script type="text/javascript">
$(document).ready(function () {
    $("#menu").treeviewMenu({
        chooseText: "Net Service",
        content: $("#dataSource").html()
    });
});
</script>
:
<div id="menu"></div>
<div id="dataSource" style="display: none;">
<ul>
    <li><a href="#">Social</a>
    <ul>
        <li><a href="#">Facebook</a></li>
        <li><a href="#">Myspace</a></li>
        <li><a href="#">Twitter</a></li>
    </ul>
    </li>
    <li><a href="#">Search</a>
    <ul>
        <li><a href="#">Google</a>
        <ul>
            <li><a href="#">Google Map</a></li>
            <li><a href="#">Google Code</a></li>
        </ul>
        </li>
        <li><a href="#">Yahoo</a></li>
    </ul>
    </li>
</ul>
</div>
```

## Options ##
  * **chooseText** `(String), Defualt: "(Choose an option)"`
> > Default text shown in the selected area.
  * **collapsed** `(Boolean), Default: true`
> > Whether the treeview nodes are collapsed or not, as default.
  * **zIndex** `(Integer), Default: 100`
> > The z-index attribute value of the treeview-menu.
  * **content** `(String), Defualt: (Emtpy)`
> > The content of the treeview. See [jquery-treeview](http://bassistance.de/jquery-plugins/jquery-plugin-treeview/).

## Methods ##

### getSelection ###
```
.treeviewMenu("getSelection")
```

> Get the selection object.

> #### Returns ####
> > `(Object)`<br />
> > (obj).value: The id attribute of the selected option.<br />
> > (obj).text: The text of the selected option.

### setSelection ###
```
.treeviewMenu("setSelection", obj)
```

> Set the selection.

> #### Arguments ####
    * **obj** `(Object)`
> > > (obj).value: The id attribute of the selected option.<br />
> > > (obj).text: The text of the selected option.


> #### Returns ####
> > `(jQuery)`