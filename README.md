# -JavaScript-
<html>
    <head>
      <meta charset="utf-8">
      <title>IFE Javascript Task 01</title>
      <style>
        p{
        	font-family: "helvetica neue", helvetica, sans-serif;
            letter-spacing: 1px;
            text-transform: uppercase;
            text-align: center;
            border: 2px solid rgba(0,0,200,0.6);
            background: rgba(0,0,200,0.6);
            box-shadow: 1px 1px 2px rgba(0,0,200,0.4);
            border-radius: 10px;
            padding: 3px 10px;
            display: inline-block;
            cursor: pointer;

        }
      </style>
    </head>
<body>
	
	
<button>Click me</button>
</body>
	<script>

//Function: creates a new paragraph and append it to the bottom of the HTMl
	function createParagraph() {
		var para = document.createElement("p");
		para.textContent = "You clicked the button!";
		document.body.appendChild(para);

	}
/*
  1. Get references to all the buttons on the page and soter them in an array.
  2. Loop through all the buttons and add a click event listener to each one.

  When any button is pressed, the createParagraph() function will be run.
*/
	var buttons = document.querySelectorAll("button");

	for(var i = 0; i < buttons.length ; i++) {
		buttons[i].addEventListener('click', createParagraph);
	}
	</script>
</html>
