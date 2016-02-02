# Google Chrome Console Commands
Interesting *Google Chrome* developer tools commands.

Editing
<table>
    <tr><td>Command</td><td>Description</td></tr>
    <tr><td>`document.body.contentEditable = true`</td><td>Make web page editable</td></tr>
</table>

Select DOM elements
<table>
    <tr><td>Command</td><td>Description</td></tr>
    <tr><td>`$(<identifier>)`</td><td>Returns first matching identifier</td>
    <tr><td>`$$(<identifier>)`</td><td>Returns all matching identifiers</td></tr>
    <tr><td>`$x(<xPath>)`</td><td>Returns array of XPath matches</td></tr>
</table>

Console Commands
<table>
    <tr><td>Command</td><td>Description</td></tr>
    <tr><td>`console.assert($("body").childNodes<1, "no content")`</td><td>Assertions</td></tr>
    <tr><td>`console.table([{a:1, b:2, c:3}, {a:"foo", b:false, c:undefined}]);`</td><td>Displays an array</td></tr>
    <tr><td>`console.log("%s has %d points", "Sam", 100);`<br>
    `console.warn("Node count:", a.childNodes.length)`<br>
    `console.error("Node count:", a.childNodes.length)`<br></td><td>Log statements</td></tr>
    <tr><td>`console.count("Init called " + user);`</td><td>Count execution</td></tr>
    <tr><td>`dir(<element>)`</td><td>View object<br>dir($("body"))</td></tr>
    <tr><td>`inspect(<element>)`</td><td>Inspect element in Elements view</td></tr>
</table>

Events
<table>
    <tr><td>Command</td><td>Description</td></tr>
    <tr><td>`monitorEvents(<element>, <event>);`<br>
    `unmonitorEvents(<element>, <event>);`</td><td>Monitor events<br>`monitorEvents(document.body, "click");`<br>
    `unmonitorEvents(document.body, "click");`</td></tr>
</table>

Profiling
<table>
    <tr><td>Command</td><td>Description</td></tr>
    <tr><td>`console.time("Array initialize");`<br>
    `console.timeEnd("Array initialize");`</td><td>Performance measurement</td></tr>
    <tr><td>`profile(<name>)`<br>
    `profileEnd(<name>)`</td><td>CPU profiling</td></tr>
    </table>

# Reference
[Using the Console](https://developer.chrome.com/devtools/docs/console#measuring-how-long-something-takes)
[15 tricks to master Chrome Developer Tools Console](https://www.youtube.com/watch?v=2zmUSoVMyRU)
