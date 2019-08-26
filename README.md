
//Foncion 1 
let blop = document.getElementsByTagName('footer')
	blop[0].addEventListener("click", function(){ 
		console.log('clique');
});

//--------------------------------------------------------------------------------------//

//Fonction 1 bis 

let footer = document.getElementsByTagName("footer");
nbClick = 0;

footer[0].addEventListener("click", function(){
    console.log("clique n°" + (nbClick += 1));
});

//----------------------------------------------------------------------------------------//

//Fonction 2
var p1 = document.querySelector('.navbar-toggler')
var p2 = document.getElementById('navbarHeader')
var unCollapseStatus = false;

	function unCollapse (){
		if (unCollapseStatus === false){
		p2.classList.remove("collapse");
		unCollapseStatus = true;
	} else {
		p2.classList.add("collapse")
		unCollapseStatus = false;
	}
};
	

p1.addEventListener("click", unCollapse);

//---------------------------------------------------------------------------------//
//Fonction 3

var p3 = document.getElementsByClassName('btn btn-sm btn-outline-secondary')
p3[0].addEventListener('click',function(){
	this.style.color ='red'
});

//-----------------------------------------------------------------------------------//
//Fonction 4
var p3 = document.getElementsByClassName('btn btn-sm btn-outline-secondary')
p3[1].addEventListener('click',function(){
	if (this.style.color ===''){
		this.style.color = 'green'
	} else {
		this.style.color = ''
	}
});


//----------------------------------------------------------------------------------------_//
//Fonction 5
var selectNavaBar = document.querySelector('header')
var polo = document.styleSheets[0]

polo.disabled = false

selectNavaBar.addEventListener('dblclick',function(){
	polo.disabled = !polo.disabled;

});

//----------------------------------------------------------------------------------------//
//Fonction 6

let p4 = document.getElementsByClassName('btn btn-sm btn-success')

p4[2].addEventListener('mouseover',function (){
	this.style.width = '20%'
});
p4[2].addEventListener('mouseout',function(){
	this.style.width = ''
})

//---------------------------------------------------------------------------------------------//
//Fonction 7

let p5 = document.getElementsByClassName('row')[1]
let p6 = document.getElementsByClassName('col-md-4')
let flech = document.getElementsByClassName('btn btn-secondary my-2')[0]

flech.addEventListener('click',function(){
	p5.insertBefore(p6[p6.length - 1], p6[0]) 

});






























