# import-Xlsx-file-in-database

/*<?php
	SimpleXLSX php class 
	MS Excel 2007 workbooks reader

  Example 1: 
	$xlsx = new SimpleXLSX('test.xlsx');
	print_r( $xlsx->rows() );
	foreach($xlsx->rows() as $rows){
  //Do something here...
  }
  Example 2:
	$xlsx = new SimpleXLSX('test.xlsx');
	if ($xslx->success())
		print_r( $xlsx->rows() );
	else
		echo 'xlsx error: '.$xslx->error();
  Example 3:
	$xslx = new SimpleXLSX( file_get_contents('http://www.test.com/test.xlsx'), true);
	list($num_cols, $num_rows) = $xlsx->dimension(2);
	echo $xlsx->sheetName(2).':'.$num_cols.'x'.$num_rows;
