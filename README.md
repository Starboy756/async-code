# async-code
//synchronus code executes code line by line

//Asynchronus allows multiple operation concurrently
//           handled with: promises,callbacks,async/await

function func1(callback){
    setTimeout(() => {console.log("This is task force 1") ; callback()},3000)
}

function func2(){
    console.log(`task force 2`)
    console.log(`task force 3`)
    console.log(`task force 4`)
    console.log(`task force 5`)
}

func1(func2);
