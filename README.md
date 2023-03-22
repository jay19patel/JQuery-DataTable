# JQuery-DataTable
![Capture](https://user-images.githubusercontent.com/107461719/226823850-c408973f-e6d8-45f2-8b46-0b3de2cf450e.PNG)


## Create html file
- create basic html home page
- add table tag in body 
- Give Id to Table tag 
- Add table head and Table Row for tile row  using api keys 
ex :
```
     <table id="example">
            <thead>
                <tr>
                    <th>Name</th>
                    <th>age</th>     
                </tr>
            </thead>
    </table>



## Javascript :
- add jquery file and css in home html page 
- add datatable cdn in home page 

- create a js file :
    - create function  for fetch api 
    - in the result consol use datatable jquery

        $(document).ready(function () {
                        var table = $('#example').DataTable({
                            "data" :result.aaData,
                            "columns": [
                                { data: "nanme" },
                                { data: "age" },
                              ]
                              #here some configratios
                        })
 
- if we need some Coustom html tags in Data table  then edit in columns data like :
        

        { data: "profile_pic" , 
          "render": function(data){
            return "<a href='"+data+"'><img src='" + data + "' height='30' alt='Image'></a>";}
        },

         
