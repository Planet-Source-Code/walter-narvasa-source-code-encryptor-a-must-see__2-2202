<div align="center">

## SOURCE CODE ENCRYPTOR \( A MUST SEE\!\!\)


</div>

### Description

IF YOU WANT TO ENCRYPT YOUR WEB PAGES OR ".JS" FILES THIS IS THE CODE FOR YOU!! THIS IS A MUST TO ALL WEB PROGRAMMERS TO PROTECT YOUR OWN WEB PAGE(S). DONT FORGET TO VOTE FOR THIS CODE!!!
 
### More Info
 
CUT AND PASTE THIS CODE AND SAVE IT INTO HTML FILE.

IF YOU TRY TO USE THIS, TRY TO ENCRYPT LINE BY LINE OF YOUR CODE AT A TIME AND NOT THE WHOLE THING AT THE SAME TIME FOR YOUR WEB PAGE TO RUN/WORK PROPERLY.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Walter Narvasa](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/walter-narvasa.md)
**Level**          |Advanced
**User Rating**    |3.4 (27 globes from 8 users)
**Compatibility**  |Java \(JDK 1\.1\), Java \(JDK 1\.2\)
**Category**       |[Security](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/security__2-74.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/walter-narvasa-source-code-encryptor-a-must-see__2-2202/archive/master.zip)

### API Declarations

```
<html>
<head>
<title>SOURCE CODE ENCRYPTOR</title>
</head>
<script>
var i=0;
var ie=(document.all)?1:0;
var ns=(document.layers)?1:0;
function initStyleElements() /* Styles for Buttons Init */
	{
		var c = document.pad;
		if (ie)
			{
				//c.text.style.backgroundColor="#DDDDDD";
				c.compileIt.style.backgroundColor="#C0C0A8";
				c.compileIt.style.cursor="hand";
				c.select.style.backgroundColor="#C0C0A8";
				c.select.style.cursor="hand";
				c.view.style.backgroundColor="#C0C0A8";
				c.view.style.cursor="hand";
				c.retur.style.backgroundColor="#C0C0A8";
				c.retur.style.cursor="hand";
				c.clear.style.backgroundColor="#C0C0A8";
				c.clear.style.cursor="hand";
			}
		else return;
	}
/* Buttons Enlightment of "Compilation" panel */
function LightOn(what)
	{
		if (ie) what.style.backgroundColor = '#E0E0D0';
		else return;
	}
function FocusOn(what)
	{
		if (ie) what.style.backgroundColor = '#EBEBEB';
		else return;
	}
function LightOut(what)
	{
		if (ie) what.style.backgroundColor = '#C0C0A8';
		else return;
	}
function FocusOff(what)
	{
		if (ie) what.style.backgroundColor = '#DDDDDD';
		else return;
	}
/* Buttons Enlightment of "Compilation" panel */
function generate() /* Generation of "Compilation" */
	{
		code = document.pad.text.value;
		if (code)
			{
				document.pad.text.value='Compiling...Please wait!';
				setTimeout("compile()",1000);
			}
		else alert('First enter something to compile and then press CompileIt')
	}
function compile() /* The "Compilation" */
	{
		document.pad.text.value='';
		compilation=escape(code);
		document.pad.text.value="<script>\n<!--\ndocument.write(unescape(\""+compilation+"\"));\n//-->\n<\/script>";
		i++;
		if (i=1) alert("Page compiled 1 time!");
		else alert("Page compiled "+i+" times!");
	}
function selectCode() /* Selecting "Compilation" for Copying */
	{
		if(document.pad.text.value.length>0)
			{
				document.pad.text.focus();
				document.pad.text.select();
			}
		else alert('Nothing for be selected!')
	}
function preview() /* Preview for the "Compilation" */
	{
		if(document.pad.text.value.length>0)
			{
				pr=window.open("","Preview","scrollbars=1,menubar=1,status=1,width=700,height=320,left=50,top=110");
				pr.document.write(document.pad.text.value);
			}
		else alert('Nothing for be previewed!')
	}
function uncompile() /* Decompiling a "Compilation" */
	{
		if (document.pad.text.value.length>0)
			{
				source=unescape(document.pad.text.value);
				document.pad.text.value=""+source+"";
			}
		else alert('You need compiled code to uncompile it!')
	}
// -->
</script>
<table border=0 width=100% cellspacing=0 cellpadding=0>
<tr>
<td width=100%>
<!-- Compilation Panel -->
<form method=post name=pad align=center>
<textarea rows=11 name=text cols=58 style="background-color:#EBEBEB;width:95%"></textarea><br>
<input type=button value=Encrypt name=compileIt onClick=generate() onMouseOver=LightOn(this) onMouseOut=LightOut(this)>
<input type=button value=Select name=select onClick=selectCode() onMouseOver=LightOn(this) onMouseOut=LightOut(this)>
<input type=button value=Preview name=view onClick=preview() onMouseOver=LightOn(this) onMouseOut=LightOut(this)>
<input type=button value=Source name=retur onClick=uncompile() onMouseOver=LightOn(this) onMouseOut=LightOut(this)>
<input type=reset value=Clear name=clear onMouseOver=LightOn(this) onMouseOut=LightOut(this)>
</form>
<!-- Compilation Panel -->
</body>
</html>
```


### Source Code

```
<html>
<head>
<title>SOURCE CODE ENCRYPTOR</title>
</head>
<script>
var i=0;
var ie=(document.all)?1:0;
var ns=(document.layers)?1:0;
function initStyleElements() /* Styles for Buttons Init */
	{
		var c = document.pad;
		if (ie)
			{
				//c.text.style.backgroundColor="#DDDDDD";
				c.compileIt.style.backgroundColor="#C0C0A8";
				c.compileIt.style.cursor="hand";
				c.select.style.backgroundColor="#C0C0A8";
				c.select.style.cursor="hand";
				c.view.style.backgroundColor="#C0C0A8";
				c.view.style.cursor="hand";
				c.retur.style.backgroundColor="#C0C0A8";
				c.retur.style.cursor="hand";
				c.clear.style.backgroundColor="#C0C0A8";
				c.clear.style.cursor="hand";
			}
		else return;
	}
/* Buttons Enlightment of "Compilation" panel */
function LightOn(what)
	{
		if (ie) what.style.backgroundColor = '#E0E0D0';
		else return;
	}
function FocusOn(what)
	{
		if (ie) what.style.backgroundColor = '#EBEBEB';
		else return;
	}
function LightOut(what)
	{
		if (ie) what.style.backgroundColor = '#C0C0A8';
		else return;
	}
function FocusOff(what)
	{
		if (ie) what.style.backgroundColor = '#DDDDDD';
		else return;
	}
/* Buttons Enlightment of "Compilation" panel */
function generate() /* Generation of "Compilation" */
	{
		code = document.pad.text.value;
		if (code)
			{
				document.pad.text.value='Compiling...Please wait!';
				setTimeout("compile()",1000);
			}
		else alert('First enter something to compile and then press CompileIt')
	}
function compile() /* The "Compilation" */
	{
		document.pad.text.value='';
		compilation=escape(code);
		document.pad.text.value="<script>\n<!--\ndocument.write(unescape(\""+compilation+"\"));\n//-->\n<\/script>";
		i++;
		if (i=1) alert("Page compiled 1 time!");
		else alert("Page compiled "+i+" times!");
	}
function selectCode() /* Selecting "Compilation" for Copying */
	{
		if(document.pad.text.value.length>0)
			{
				document.pad.text.focus();
				document.pad.text.select();
			}
		else alert('Nothing for be selected!')
	}
function preview() /* Preview for the "Compilation" */
	{
		if(document.pad.text.value.length>0)
			{
				pr=window.open("","Preview","scrollbars=1,menubar=1,status=1,width=700,height=320,left=50,top=110");
				pr.document.write(document.pad.text.value);
			}
		else alert('Nothing for be previewed!')
	}
function uncompile() /* Decompiling a "Compilation" */
	{
		if (document.pad.text.value.length>0)
			{
				source=unescape(document.pad.text.value);
				document.pad.text.value=""+source+"";
			}
		else alert('You need compiled code to uncompile it!')
	}
// -->
</script>
<table border=0 width=100% cellspacing=0 cellpadding=0>
<tr>
<td width=100%>
<!-- Compilation Panel -->
<form method=post name=pad align=center>
<textarea rows=11 name=text cols=58 style="background-color:#EBEBEB;width:95%"></textarea><br>
<input type=button value=Encrypt name=compileIt onClick=generate() onMouseOver=LightOn(this) onMouseOut=LightOut(this)>
<input type=button value=Select name=select onClick=selectCode() onMouseOver=LightOn(this) onMouseOut=LightOut(this)>
<input type=button value=Preview name=view onClick=preview() onMouseOver=LightOn(this) onMouseOut=LightOut(this)>
<input type=button value=Source name=retur onClick=uncompile() onMouseOver=LightOn(this) onMouseOut=LightOut(this)>
<input type=reset value=Clear name=clear onMouseOver=LightOn(this) onMouseOut=LightOut(this)>
</form>
<!-- Compilation Panel -->
</body>
</html>
```

