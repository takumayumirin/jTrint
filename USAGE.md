# Print Responsively – Usage

```
<script type="text/javascript" src="print-responsively.js"></script>
<link rel="stylesheet" type="text/css" href="print-responsively.css" />
<script>
$(function() {
	printResponsively(options);
});
</script>
```

## Configuration

<table width="100%">
    <tr>
        <th align="left" colspan="5"><a href="#prerequisite-classes" name="prerequisite-classes">Prerequisite Classes</a></th>
    </tr>
	<tr>
		<th align="left" colspan="1">Class</th>
		<th align="left" colspan="2">Description</th>
		<th align="left" colspan="2">Prerequisite</th>
	</tr>
    <tr>
        <td><code>.hide-print</code></td>
        <td colspan="2">This will hide the visible element on print.</td>
        <td colspan="2"></td>
    </tr>
    <tr>
        <td><code>.show-print</code></td>
        <td colspan="2">This will show the hidden element on print.</td>
        <td colspan="2"></td>
    </tr>
    <tr>
        <td><code>.header-area</code></td>
        <td colspan="2">Place this class in the parent container of the header where its associated contents are also included. You may combine this class with <code>.footer-area</code> class if there's also a footer incorporated.</td>
        <td colspan="2"><code>header</code></td>
    </tr>
    <tr>
        <td><code>.footer-area</code></td>
        <td colspan="2">Place this class in the parent container of the footer where its associated contents are also included. You may combine this class with <code>.header-area</code> class if there's also a header incorporated.</td>
        <td colspan="2"><code>footer</code></td>
    </tr>
    <tr>
        <th align="left" colspan="5"><a href="#options" name="options">Options</a></th>
    </tr>
	<tr>
		<th align="left" width="20%">Option</th>
		<th align="left" width="40%">Description</th>
		<th align="left" width="10%">Prerequisite</th>
		<th align="left" width="10%">Type</th>
		<th align="left" width="10%">Default</th>
	</tr>
    <tr>
        <td><code>buttonClass</code></td>
        <td>Allows the user to add more classnames to the print button. For multiple class, add space as delimiter just like inputting classes in HTML.</td>
        <td><code>buttonContainer</code></td>
        <td><code>string</code></td>
        <td></td>
    </tr>
    <tr>
        <td><code>buttonContainer</code></td>
        <td>A required option if the user wanted to place a print button. Pass it with node name, id (<code>#id</code>) of the element or class (<code>.class</code>) of the element/s if you like to put the print button in multiple places of your page.</td>
        <td></td>
        <td><code>string</code></td>
        <td></td>
    </tr>
    <tr>
        <td><code>buttonText</code></td>
        <td>Allows the user to change the default text of the print button. You may also add the size name by adding <code>&lt;size&gt;</code> in the string. This option is recommended if you have multiple page sizes.</td>
        <td><code>buttonContainer</code></td>
        <td><code>string</code></td>
        <td>Print</td>
    </tr>
    <tr>
        <td><code>container</code></td>
        <td>Assigns a container element to be the only content to be shown on print. For multiple containers, add comma as delimiter. Please be sure to include selector.</td>
        <td></td>
        <td><code>string</code></td>
        <td><code>body</code></td>
    </tr>
    <tr>
        <td><code>cssContainer</code></td>
        <td>Specifies the container where the dynamically added css file will be placed. The default would be in the first <code>head</code> of the document. If there's no <code>cssPath</code> but the user placed this option, it will occur an error.</td>
        <td><code>cssPath</code></td>
        <td><code>string</code></td>
        <td><code>head</code></td>
    </tr>
    <tr>
        <td><code>cssPath</code></td>
        <td>This is used for dynamically adding of the css file of Print Responsively by passing its file or url path.</td>
        <td></td>
        <td><code>string</code></td>
        <td></td>
    </tr>
    <tr>
        <td><code>footer</code></td>
        <td>Assigns a container element to be the footer of the page on print. There should be one for each <code>.footer-area</code>.</td>
        <td><code>.footer-area</code></td>
        <td><code>string</code></td>
        <td></td>
    </tr>
    <tr>
        <td><code>header</code></td>
        <td>Assigns a container element to be the header of the page on print. There should be one for each <code>.header-area</code>.</td>
        <td><code>.header-area</code></td>
        <td><code>string</code></td>
        <td></td>
    </tr>
    <tr>
        <td><code>keypress</code></td>
        <td>If true, it will allow the user to print using <kbd>ctrl</kbd> and <kbd>P</kbd> with the configured layout.</td>
        <td></td>
        <td><code>boolean</code></td>
        <td><code>false</code></td>
    </tr>
    <tr>
        <td><code>margin</code></td>
        <td>Specifies the margin for all pages. Pass margin the same way in css. There are still no function where the user can change margin on multiple pages.</td>
        <td></td>
        <td><code>string</code></td>
        <td>0</td>
    </tr>
    <tr>
        <td><code>orientation</code></td>
        <td>Allows the user to change the layout of the pages. There are only two choices for this option: portrait and landscape.</td>
        <td></td>
        <td><code>string</code></td>
        <td>portrait</td>
    </tr>
    <tr>
        <td><code>size</code></td>
        <td>Allows the user to change the paper size and add more wih delimiter comma. If the desired size is not in the list, you may add manual size e.g. <code>&lt;120cmX130cm&gt;</code> in widthXheight format. The measurements should be in lowercase and the delimiter 'X' should be in uppercase.</td>
        <td></td>
        <td><code>string</code></td>
        <td>letter</td>
    </tr>
</table>