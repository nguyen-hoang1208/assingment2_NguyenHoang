# assingment2_NguyenHoang
//In server.js, we use the method GET/POST/PUT/DELETE. 
//However, we need to include express module such as using listening, express static to include the file html into current
working space and using body Parse to wrap these value inputs in scripts.js
   const express=require('express');                       
   const app=express();                                 
   const fs=require('fs');                              
   var bodyParser= require('body-parser');
   app.listen(3000,()=>console.log('listening at 3000')); 
   app.use(express.static(__dirname));                   
   app.use(bodyParser.json());        
These GET/POST/PUT/DELETE will be provided in this file:
       app.get('/arrayof3Items', function(req,res){    
       }) 
       app.post('/arrayof3Items',function(req,res){
       })
      app.put('/arrayof3Items/:id',function(req,res){   
       })
      app.delete('/arrayof3Items/:id',function(req,res){
    )  
      We use jQuery in Script.js file via these methods to perform select form for submitting, click on button.
    $('#get-button').on('click',function() to click button link to inde.html
     $.ajax with these default set up        
     tbodyEl.html('') to append these field of table tbodyEl.append
     For put:
     $('#create-form').on('submit',function(event) to create submit button and using event.preventDefault 
     to prevent the submit page, data is stringify via JSON.stringify method 
     For update:
   $('table').on('click','.update-button',function() to select any button update appropriate with the row then 
      using rowEl function to wrap all fields rowEl.find('.id').text();       
     For delete:
    $('table').on('click','.delete-button',function() to select the button on delete, using rowel method
        var rowEl=$(this).closest('tr');
        var id=rowEl.find('.id').text();
        $.ajax  method:'DELETE',
