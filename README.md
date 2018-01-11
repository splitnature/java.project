# java.project
//java file for school project
/created A Function named idcard
function IDcard(){


  var FirstName=document.getElementById("FirstName").value;
  var LastName=document.getElementById("LastName").value;
  var Address=document.getElementById("Address").value;
 //created 3 variables that pulls the value of each input

       document.getElementById("postFullName").innerHTML=FirstName+LastName;
       document.getElementById("postAddress").innerHTML=Address;
       //used DOM innerhtml to post first and last name to the tag that has an id of postfullname inside the id card
        //used DOM innerhtml to post Adress to the tag that has an id of postAddress inside the id card

  var age=parseInt(document.getElementById('Age').value);
  var phoneNumber=parseInt(document.getElementById('PhoneNumber').value);
  //created two  variables  age and number pulling the value of the corresponding input using DOM

       var numberArrray=[];//created empty array named numberArrray

              numberArrray.push(age,phoneNumber);
               //pushed both age and phone number into the empty array using push() method


      for (var i=0; i<numberArrray.length;i++){

                                                      //created a for loop through numberArrray
            if (numberArrray[i]<=100)   {
               document.getElementById('postAge').innerHTML="Age:"+ age;
            }

       else if (numberArrray[i]>100) {
           document.getElementById('postPhoneNumber').innerHTML="Phone Number:"+ phoneNumber;

       }

     }

   }
