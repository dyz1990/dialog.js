# dialog.js
html5 dialog to replace window.alert/confirm/prompt

# Install

`npm i --save @dyz1990/dialog.js`

OR

 ` <script src="dialog.js"></script>`

# usage

 ```
<script>
//Alert
dialog.alert('Message')
//Or
dialog.alert('Title','Message')

//Confirm
dialog.confirm('Title','Message')
.then(function(){
  //do confirm
})
.catch(function(){
  //to cancel
})

//Prompt
dialog.prompt("Title", "label","default value")
.then(value=>{
  console.log('input value is ', value)
})
.catch(()=>{
  //cancelled
})
</script>
 ```