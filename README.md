# datatables-folder
# how to implement datatables in code

<head>
    <link href="css/ie10-viewport-bug-workaround.css" rel="stylesheet"> //check optional r not
    <script src="js/ie-emulation-modes-warning.js"></script>           //check optional r not

    <link href="js/datatables/bootstrap.min.css" rel="stylesheet">
		<link rel="stylesheet"  href="js/datatables/dataTables.bootstrap4.min.css" />
		<link rel="stylesheet"  href="js/datatables/buttons.bootstrap4.min.css" />
</head>


//footer
<script src="js/datatables/Bootstrap.min.js"></script>
	  <!--data tables-->
	    
		<script src="js/datatables/jquery.dataTables.min.js"></script>
		<script src="js/datatables/dataTables.bootstrap.min.js"></script>
		<script src="js/datatables/dataTables.buttons.min.js"></script>
		<script src="js/datatables/buttons.bootstrap.min.js"></script>
		<script src="js/datatables/jszip.min.js"></script>
		<script src="js/datatables/pdfmake.min.js"></script>
		<script src="js/datatables/vfs_fonts.js"></script>
		<script src="js/datatables/buttons.html5.min.js"></script>
		<script src="js/datatables/buttons.print.min.js"></script>
		<script src="js/datatables/buttons.colVis.min.js"></script>
   
	  <script>
  <script>
	 $(document).ready(function() {
         var table = $('#example').DataTable( {
         lengthChange: false,
         buttons: [ 
                    {
                    extend: 'excel',
                    
                    },
                    {
                    extend: 'pdfHtml5',
                    orientation: 'landscape',
                    pageSize: 'A0'
                    },
                    {
                    extend: 'colvis',
                   
                    }
                ],
         } );
 
    table.buttons().container()
        .appendTo( '#example_wrapper .col-sm-6:eq(0)' );
} );
	  </script>
