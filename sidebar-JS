var stickynav = moveNav(".manage-beacons",".footer",".sticky",200,true);

function moveNav(upperElement,lowerElement,nav,offsetY) {	

	$( window ).scroll(function() {
		
		minY = $(upperElement).offset().top;
		maxY = $(lowerElement).offset().top;
		
		curY = $(window).scrollTop();

		if (curY > (minY-offsetY) && curY < maxY){
			$( nav ).css({
				"position" : "fixed",
				"top" : offsetY
			});
		}else{
			$( nav ).css({
				"position" : "absolute",
				"top" : minY
			});			
		}
	})
}