# probable-lamp
$im=imagecreate(500,500);//创建图形500*500  

$black=imagecolorallocate($im,0,0,0);  

$red=imagecolorallocate($im,255,0,0);//设置图形颜色  

imagepolygon($im,$str,360,$red);  

imagestring($im,5,190,190,"love",$red);//输出字符串  

header('Content-type:image/gif');//通知浏览器输出的是gif图片  

imagegif($im);//输出图片  

imagedestroy($im);//销毁  

?>  
