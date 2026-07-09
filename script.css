let display = document.getElementById("display");
let historyList = document.getElementById("historyList");

let memory = 0;

function append(val){
    display.value += val;
}

function clearDisplay(){
    display.value = "";
}

function deleteLast(){
    display.value = display.value.slice(0,-1);
}

function calculate(){
    try{
        let result = eval(display.value);
        addHistory(display.value + " = " + result);
        display.value = result;
    }
    catch{
        display.value = "Error";
    }
}

function addHistory(text){
    let li = document.createElement("li");
    li.textContent = text;
    historyList.appendChild(li);
}

function sqrt(){
    display.value = Math.sqrt(display.value);
}

function power(){
    display.value = Math.pow(display.value,2);
}

function log(){
    display.value = Math.log10(display.value);
}

function sin(){
    display.value = Math.sin(display.value);
}

function cos(){
    display.value = Math.cos(display.value);
}

function tan(){
    display.value = Math.tan(display.value);
}

function memoryAdd(){
    memory += Number(display.value);
}

function memorySub(){
    memory -= Number(display.value);
}

function memoryRecall(){
    display.value = memory;
}

function memoryClear(){
    memory = 0;
}

document.addEventListener("keydown",function(e){

    if(!isNaN(e.key) || "+-*/.".includes(e.key)){
        append(e.key);
    }

    if(e.key==="Enter"){
        calculate();
    }

    if(e.key==="Backspace"){
        deleteLast();
    }

});
