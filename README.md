<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>TO DO LIST</title>
    <link href="assets/css/style.css" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
  </head>
  <body>
    <div id="container">
      <h1>TO DO LIST<i class="fa fa-plus"></i></h1>
      <input type="text" name="text" placeholder="Add Do List">
      <ul>
        <li><span><i class="fa fa-trash"></i></span> GO TO HELL</li>
        <li><span><i class="fa fa-trash"></i></span> Go to school</li>
        <li><span><i class="fa fa-trash"></i></span> Go to lord</li>
      </ul>
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js" type="text/javascript"></script>
    <script src="assets/js/style.js" type="text/javascript"></script>
  </body>
</html>

style.css
@import url('https://fonts.googleapis.com/css?family=Roboto:400,700');

body {
  font-family: 'Roboto',sans-serif;  
  background: #B2FEFA;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #0ED2F7, #B2FEFA);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #0ED2F7, #B2FEFA); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

}

.completed {
  color: gray;
  text-decoration: line-through;
}

#container {
  margin: 0 auto;
  width: 400px;
  box-shadow: 2px 2px 2px 1px rgba(0, 0, 0, 0.2);
  background-color: #fff;
}

h1 {
  background-color: #3498db;
  margin: 0;
  padding: 10px;
  color:white;
  font-weight: normal;
  font-size: 30px;
}

.fa-plus {
  float: right;
}

input[type=text]{
  width: 100%;
  padding: 15px 15px 15px 20px;
  color: #3498db;
  font-size: 25px;
  box-sizing: border-box;
  background-color: #ecf0f1;
  border: 3px solid rgba(0,0,0,0);
}

input:focus {
  border: 1px solid #3498db;
}

ul {
  margin: 0;
  list-style: none;
  padding: 0;
}

li {
  background-color: #fff;
  height: 40px;
  line-height: 40px;
  cursor: pointer;
}

li:nth-child(2n){
  background-color: #ecf0f1;
}

span {
  width: 0px;
  color: #fff;
  background-color: #e74c3c;
  display: inline-block;
  text-align: center;
  margin-right: 20px;
  transition: 0.5s;
  opacity: 0.5;
}

li:hover span {
  width: 40px;
  transition: 0.5s;
  opacity: 1.0;
}
