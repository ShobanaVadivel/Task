//Object

var obj={"person":murali, "age":36, "company":"saipem"}
for(var i in obj){
console.log(i); //give key as output
console.log(obj[i]); //give value as output
}


// Array of Objects

var obj=[{"person":"murali", "age":38, "company":"saipem"},
{"person":"arul", "age":36, "company":"saipem1"},
{"person":"srini", "age":31, "company":"saipem2"}]

for(var i in obj){
console.log(i); // it will give index value of array of objects
console.log(obj[i]); //it will print each object as out put
console.log(obj[i].person,obj[i].age,obj[i].company); // printing all vaues of keys
}

var obj=[{"person":"murali", "age":38, "company":"saipem"},
{"person":"arul", "age":36, "company":"saipem1"},{"person":"srini", "age":31, "company":"saipem2"}]
for(var i in obj){
for(var j in obj[i])  {                                                                                                                                                              console.log(j+":"+obj[i][j]); // person:murali format}
}

//API
set of business logic to interact with other software.

//Ajax
var xhr=new XMLHttpRequest();
xhr.open('GET','API URL');
xhr.onload= function(){
var data=JSON.parse(this.response);
console.log(data);
};
xhr.send();
<<-->>cors-cross origin resource sharing(it will give data to every users if cors is there)

