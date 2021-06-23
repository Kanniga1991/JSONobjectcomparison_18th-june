# JSONobjectcomparison_18th-june

var obj1 = {"name":"Sam","class":"MCA"};
var obj2 = {"class":"MCA","name":"Sam"};

var flag=true;

if(Object.keys(obj1).length==Object.keys(obj2).length){
    for(key in obj1) { 
        if(obj1[key] == obj2[key]) {
            continue;
        }
        else {
            flag=false;
            break;
        }
    }
}
else {
    flag=false;
}
console.log("is object equal"+flag);


const object1={
name:'ABC',
address:'India'
}

const object2={
address:'India',
name:'ABC'
}

JSON.stringify(object1)===JSON.stringify(object2)
// false

_.isEqual(object1, object2)
//true
