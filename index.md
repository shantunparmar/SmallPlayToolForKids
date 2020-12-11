<html>
    <head>
        <link rel="stylesheet" href="bsls-ui.css">
        <script src="bsls-presentation.js"></script>
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/css/bootstrap.min.css">
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/js/bootstrap.min.js"></script>
</head>
    <body>
        
        <div class="container-fluid">
             <div class="row">
               <div class="col-md-12">
                   <img src="BSLS.gif"/>
               </div>
            </div>
            
            <div class="row">
               <div class="col-md-12">
                   <h2>Learning Tool (ver 1)</h2>
               </div>
            </div>
            
            <div class="row">
                <div class="form-group col-md-6">
                    No. of Cols : 
                    <input type="number" class="form-control" min="1" max="100" name="cols" id="cols" required value="3"/>
                </div>
                <div class="form-group col-md-6">
                    No. of Rows : 
                    <input type="number" class="form-control" min="1" max="100" name="rows" id="rows" required value="3"/>
                </div>
                
                <div class="form-group col-md-6">
                    Sample Cell Data :
                    <input type="text" class="form-control" name="data" required id="data"/>
                </div>
                <div class="form-group col-md-6">   
                    Cell Height (in pixels, Min height:40px)
                    <input type="number" class="form-control" min="1" max="50" name="height" required id="height" value="10"/>
                </div>
                
                <div class="form-group col-md-6">   
                    Cell width (in pixels, Min width:40px)
                    <input type="number" class="form-control" min="1" max="50" name="width" required id="width" value="10"/>
                </div>
                
                <div class="form-group col-md-6">
                  <label for="sel1">Select Color:</label>
                  <select class="form-control" id="color">
                    <option value="black">Black</option>
                    <option  value="white" selected>White</option>
                    <option value="red">Red</option>
                    <option value="green">Green</option>
                    <option value="blue">Blue</option>
                    <option  value="yellow">Yellow</option>
                    <option value="purple">Purple</option>
                    <option  value="cyan">Cyan</option>
                    <option value="pink">Pink</option>
                    <option value="orange">Orange</option>
                    
                    
                  </select>
                </div>
                
                <div class="form-group col-md-6">   
                    Count Down Timer
                    <input type="number" class="form-control"  name="timer" required id="timer" value="10"/>
                </div>
                <div class="form-group col-md-6">
                    <button class="btn btn-primary" onclick="clock();">Start counter</button>
                    <button class="btn btn-primary" onclick="clearInterval(myTimer);">Stop counter</button>
                </div>
                <div class="col-md-12">
                    <button type="button" class="btn btn-primary" onclick="generate()">Generate Table</button>
                    <button type="button" class="btn btn-danger" onclick="clearDom()">Clear Table</button>    
                </div>
                
            </div>
            
            <div class="row">
               <div class="form-group col-md-12" id="appData">
                    <!--<table class="" id="table">
                        <tbody id="body">
                        </tbody>
                    </table>-->
                </div>
            </div>
        </div>
    </body>
</html>
