字模数据生成.

较早写的一个小程序, 主要是给另外一个程序做数据生成用的.
使用freetype2读取数据

支持任何大部分字体, 默认直接打印出字体的图样到console, 
如果指定输出文件则输出字模数据到指定文件.

需要指定字体文件默认使用./font/wqy.tty
由于字体文件较大所以没有上传上来.

默认帮助信息
---------------------------
	This program convert letter to matrix data
	Usage: gend [OPTION]... [STRING]...
	-i, --input-file <arg>    file will used convert
	                          default used the STRING
	-o, --output-file <arg>   file will be write the matrix data
	                          default file is 'output'
	-f, --font <path>         use which font
	-s, --size <arg>          only use for display
	-q, --quiet               don't display used for shell
	-h, --help                print this help text



"./gen snyh" 的输出结果
--------------------------


	OOOOO
	O    
	O    
	OOOO 
	   OO
	   OO
	OOOO 

	OOOOO 
	OO  OO
	O   OO
	O   OO
	O   OO
	O   OO
	O   OO

	O    OO
	OO  OO 
	OO  OO 
	 OOOO  
	 OOOO  
	  OO   
	  OO   
	  OO   
	 OO    
	OO     

	O     
	O     
	O     
	O     
	OOOOO 
	OO  OO
	O   OO
	O   OO
	O   OO
	O   OO
	O   OO


输出的数据文件:
---------------

	0x78, 0x80, 0x80, 0x70, 0x08, 0x08, 0xf0, 0x00, 
	0x00, 0x00, 0x00, 0x00, 0x69, 0x82, 0x00, 0x00, 
	0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 
	0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 

	0xb8, 0xc4, 0x84, 0x84, 0x84, 0x84, 0x84, 0x00, 
	0x00, 0x00, 0x00, 0x00, 0x91, 0xf3, 0x01, 0x00, 
	0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 
	0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 

	0x82, 0x44, 0x44, 0x28, 0x28, 0x10, 0x10, 0x10, 
	0x20, 0xc0, 0x00, 0x00, 0x91, 0xf3, 0x01, 0x00, 
	0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 
	0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 

	0x80, 0x80, 0x80, 0x80, 0xb8, 0xc4, 0x84, 0x84, 
	0x84, 0x84, 0x84, 0x00, 0x91, 0xf3, 0x01, 0x00, 
	0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 
	0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 
