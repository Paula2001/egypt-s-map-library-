let data =
[ {'gov':'Alexandria' ,'desc' : "this is description",'top': 1 ,'left': 40 } ,
{'gov':'Cairo' ,'desc' : "this is description",'top': 12 ,'left': 55 },
{'gov':'Qina' ,'desc' : "this is description",'top': 51 ,'left': 65 },
{'gov': 'Portsaid','desc':"This is our Portsaid Company",'top': 1,'left': 62},
{'gov': 'Dymyat','desc':"This is our dumyat Company",'top': 3,'left': 56},
{'gov': 'Southern Sinai','desc':"descrption",'top': 20,'left': 72},
];
class Map{
    constructor(){
        this.executeCreationElements();
    }
    
    createAllElements(title_text ,description_text,top,left){
        let main = document.getElementById("map");
        let box = document.createElement("div");
        main.appendChild(box);
        box.className = "box";
        box.style.top = `${top}%` ; 
        box.style.left = `${left}%`; 
        let bin = document.createElement("div");
        bin.className = "bin"; 
        box.appendChild(bin);
        let text = document.createElement("div");
        text.className = "text"; 
        box.appendChild(text);
        let title = document.createElement('p');
        title.innerHTML = title_text ; 
        text.appendChild(title);
        let description = document.createElement('p');
        text.appendChild(description);
        description.innerHTML = description_text ; 
    }
    executeCreationElements(){
        data.forEach(gov => {
            this.createAllElements(gov['gov'],gov['desc'],gov['top'],gov['left']);
        });
    }
    
}
let map = new Map();