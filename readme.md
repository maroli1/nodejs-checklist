console.log("hello maryam, how are you")


//ساخت سرور ساده بدون اکسپرس
const http = require("http")
const server = http.createServer(
   (req,res)=>{
 res.writeHead(200,{"content-type":"text/plain"})
    res.end("سلام این یک سرور ساده با جی اس است");
    server.listen(3000,()=>{
            console.log("server is running the port 3000")
    })
});
const express = require("express");
const send = require("send");
const app = express ();
app.get( "/",(req,res)=> {"hi express.js"});
app.listen (3000,()=>
console.log(" server roy port 3000 dar hal rjra ast"))\



// نوشتن یک میدلور ساده 

const express = require("express")
const app = express ()
app.use= ((req,res,next)=>{
const express = require("express")
const app = express();
})

app.get("/",(req,res)=> {
    res.send ("hello")

});

app.listen (3000,()=>{
   console.log ("listen port 3000")
});




//متغیر 
const a = 10            //تغیر نمیکند
let b = 20             // قابل تغیر 
let name = "maryam"
let age = 22 
console.log(a,b,name,age)



//ماژول ها 
function sum (a,b)
{return a+b}
module.exports = //پوشه ی دلخواه 




// ساخت یک api یا وبسایت 

const express = require ("express")
const app = express ()
app.get ("/",(req,res)=>{
res.send("hello world")
})
app.listen (3000,()=>
console.log ("server is running"))



//میدلور ها 
//میدلوور با app.use نوشته میشه 

app.use ((req,res,next)=>     //(اگه next رو صدا نزنیم درخواست قفل میشه )
{console.log ( "درخواست از اینجا رد بشه")
    next ();
})



//روت ها    // get /post/put/delete


app.get ("/user", (req,res)=>
res.send ('get کاربر '))
app.post ("/user ",(req,res)=>
res.send ("post کاربر جدید "))
app.put ("/user",(req,res) =>
res.send ("put ویرایش کاربر "))
app.delete ("/user" , (req,res)=>
res.send ("delet حذف کاربر "))



//json ارسال     // فرستادن به فرانت 

app.get ("/json",(req,res)=>{
    res.json ({name : "maryam", age : "22"})
})


//async برای کار با عملیاتی ک زمان بر است 

function getNumber (){
    return new promise(resolve =>{
        setTimeout(() => resolve(42),2000)
  })
}
async function  run(){
const num = await getNumber();
  console.log(num);
}
    
run ();


//مدیریت خطا (میدلوور)  در اکسپرس   // هندل کردن خطاها 
app.use ((err,(req,res,next)=>
{console.log ("errore :",err.massage)
res.status(500).send("خطای داخلی سرور ")
}))

