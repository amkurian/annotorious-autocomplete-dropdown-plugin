# Annotorious Autocomplete Dropdown Plugin


A simple [Annotorious](https://github.com/annotorious/annotorious) plugin that allow users to add annotations with the autocomplete suggestion displayed as dropdown.

## Using this Plugin

Simply [download the script](https://raw.githubusercontent.com/amkurian/annotorious-autocomplete-dropdown-plugin/master/anno-autocomplete-dropdown-plugin.js),
copy it to your server/Webspace and set it up with your page as described below.

1. The plugin uses jQuery. Therefore you need to import jQuery before importing the plugin script.
2. Add the plugin script to your page just like any other Annotorious plugin. Make sure the plugin script is
   loaded __after__ the main Annotorious script.
3. Attach the plugin to Annotorious using the ``anno.addPlugin`` API method.
4. Specify the array of suggestions in `annotorious.plugin.AutocompleteDropdown.prototype._loadAnnotations` function either as static array or dynamic array.
## Example

    ....
      <head>
        <!-- Import main Annotorious script and CSS -->
        <link rel="stylesheet" href="https://annotorious.github.com/latest/annotorious.css" type="text/css" />
        <script src="https://annotorious.github.com/latest/annotorious.min.js"></script>
        
        <!-- Import jQuery -->
        <script src="jquery-1.9.0.min.js"></script>
        
        <!-- Import the plugin script -->
        <script src="my-script/sanno-autocomplete-dropdown-plugin.js"></script>
        
        <!-- Use Annotorious' JavaScript API to attach and activate the plugin -->
        <script>
          anno.addPlugin('AutocompleteDropdown');
        </script>
      <head>
    ....
    
   
