# CSS3

Created in order to format the HTML sheets for better reading.

* [MDN(Mozilla Developer Network) documentation](https://mdn.dev)

### Selectors

When you're formatting text, sometimes you don't want to make links or bolds look the same. That's why you can assign different styles by giving the HTML tags their own **id** and **class** names.

`a, p, h1, h3 {`
	`color: red;`
	`font-size: 12px;`
`}`

`.header_class {`
`	padding: 15px;`

`}`

`#header_id {`
	`padding: 10px;`
`}`

> Note: there can only be one id per page!



You *must* reference the CSS style sheet in the HTML file. Naturally, you have to do so in the **head** section.

HTML below:

<!DOCTYPE html>
    <html>
        <head>
            <meta charset="utf-8">
            <title>TITLE</title>
            <link rel="stylesheet" href="style.css">
        </head>
</html>
</!doctype>



### Style

#### Border

thickness - style - color

.post {
	border: 3px solid blue;
	border-top: 2px dotted green;
	border-right: 4px dashed pink;
	border-width: 3px;
	border-color: #CCC;
	border-style: dashed;
	border-top-width: 4px;
	border-left-color: #DDD;
	border-bottom-style: solid;
	border-radius: 50%;			// this makes the square turn into a cirlce!
	border-radius: 10px 20%;

}



#### Padding

.post {
	padding: 10px 5px; 	//the Y axis(bottom-top) will have 10px and X(left-right, 5px
	padding: 10px 5px 0 15; //top - right - bottom -left
	padding-top: 5px;
	padding-left: 3px;
}
