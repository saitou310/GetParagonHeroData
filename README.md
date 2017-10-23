# GetParagonHeroData

paragon heroes page
https://www.epicgames.com/paragon/en-US/heroes

var a = "";
$($('[data-reactid="240"] a')).each(function(i){

a = a + "," + $(this).find('.caption').children('h5').html();
a = a + "," + $(this).find('.caption').children('h6').text();
$(this).find('.traits li').each(function(j){
 a = a+"," + $(this).text();
});
console.log(a);
a = "";
});

