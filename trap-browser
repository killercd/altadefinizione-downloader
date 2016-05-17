// ==UserScript==
// @name				Content Assistant
// @namespace		http://www.github.com
// @description	Add comments to your geocaches on geocaching.com.
// @include			*copernico.wki.it*

// @grant				none
// @version			82
// @author			Groch
// ==/UserScript==


window.onload = function(){
	
    arrLink = jQuery('body').find('a');
    counter = 0;
    for (var k in arrLink) {
        counter++;
        //jQuery(arrLink[k]).text(jQuery(arrLink[k]).text+" ("+counter+")");
        if(jQuery(arrLink[k]).text().trim()!==''){
            txtLinkContent = jQuery(arrLink[k]).text();
            jQuery(arrLink[k]).text(txtLinkContent+" ("+k+")");
        }
        
        
    }
    
    //jQuery('#content').append("<div id=\"lukeDivWalker\" style=\"display:none; background-color:#d8d8d8; width:500px; height:500px; position: absolute; left: 50%;\"><div style=\"position: relative; left: -50%; border: dotted red 1px;\"></div></div>");
    
   
    
    /*
    // @require			http://code.jquery.com/jquery-latest.js
    $.each($arrLink, function(indx, val){
		console.log($(this).text());
    });*/
};

 jQuery(window).bind('keydown', function(event) {
        
        //if (event.ctrlKey || event.metaKey) {
        if (event.ctrlKey || event.shiftfKey) {
            switch (String.fromCharCode(event.which).toLowerCase()) {
                case 'l':
                    event.preventDefault();
                    jQuery('#lukeDivWalker').show();
                    break;
                
            }
        }
    });

