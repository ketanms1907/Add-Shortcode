Function.php

1./*SHortcode-1*/
add_shortcode( 'home_banner_date_and_cash', 'home_banner_date_cash' );
function home_banner_date_cash( $atts ){
ob_start();
global $cash;
$cash = $atts['cash'];
get_template_part( 'inc/inc-home-banner-date-cash' );
return ob_get_clean();
}

php File: <?php do_shortcode(['home_banner_date_and_cash']); ?>

2./*SHortcode-2*/

function bartag_func( $atts ) {
$atts = shortcode_atts(
array(
'foo' => 'no foo',
'bar' => 'default bar',
), $atts, 'bartag' );
return 'bartag: ' . $atts['foo'] . ' ' . $atts['bar'];
}
add_shortcode( 'bartag', 'bartag_func' );

o/p:[bartag foo="koala" bar="bears"]
