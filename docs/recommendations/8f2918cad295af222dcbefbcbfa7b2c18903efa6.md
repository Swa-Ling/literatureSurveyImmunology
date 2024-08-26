---
hide:
 - navigation
---
<!DOCTYPE html>
#
<html lang="en">
<head>
  <meta charset="utf-8">
</head>

<body>
  <p>
  <i class="footer">This page was last updated on 2024-08-26 06:02:00 UTC</i>
  </p>
  
  <div class="note info" onclick="startIntro()">
    <p>
      <button type="button" class="buttons">
        <div style="display: flex; align-items: center;">
        Click here for a quick intro of the page! <i class="material-icons">help</i>
        </div>
      </button>
    </p>
  </div>

  <p>
  <h3 data-intro='Recommendations for the article'>
    Recommendations for the article <i>Bispecific T cell engager therapy for refractory rheumatoid arthritis.</i>
  </h3>
  <table id="table1" class="display wrap" style="width:100%">
  <thead>
    <tr>
        <th data-intro='Click to view the abstract (if available)'>Abstract</th>
        <th>Title</th>
        <th>Authors</th>
        <th>Publication Date</th>
        <th>Journal/ Conference</th>
        <th>Citation count</th>
        <th data-intro='Highest h-index among the authors'>Highest h-index</th>
    </tr>
  </thead>
  <tbody>
    
        <tr id="[This retracts the article DOI: 10.1155/2022/9273641.].">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/55b20a0151e2288098b7c17b497132ca11b1fc33" target='_blank'>Retracted: Application of Machine Learning in Rheumatic Immune Diseases</a></td>
          <td>
            Journal of Healthcare Engineering
          </td>
          <td>2023-01-26</td>
          <td>Journal of Healthcare Engineering</td>
          <td>0</td>
          <td>2</td>
        </tr>
    
        <tr id="None">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/95bb9e5624b1117fc20e0cf3594c6504178f9585" target='_blank'>Identification</a></td>
          <td>
            C. Adams
          </td>
          <td>2010-09-01</td>
          <td>DBLP</td>
          <td>383</td>
          <td>2</td>
        </tr>
    
        <tr id="None">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/95bb9e5624b1117fc20e0cf3594c6504178f9585" target='_blank'>Identification</a></td>
          <td>
            C. Adams
          </td>
          <td>2010-09-01</td>
          <td>DBLP</td>
          <td>383</td>
          <td>2</td>
        </tr>
    
        <tr id="None">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/95bb9e5624b1117fc20e0cf3594c6504178f9585" target='_blank'>Identification</a></td>
          <td>
            C. Adams
          </td>
          <td>2010-09-01</td>
          <td>DBLP</td>
          <td>383</td>
          <td>2</td>
        </tr>
    
        <tr id="None">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/95bb9e5624b1117fc20e0cf3594c6504178f9585" target='_blank'>Identification</a></td>
          <td>
            C. Adams
          </td>
          <td>2010-09-01</td>
          <td>DBLP</td>
          <td>383</td>
          <td>2</td>
        </tr>
    
        <tr id="[This retracts the article DOI: 10.1155/2022/5162768.].">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/98a4e8f3ae8a013ba4c81b2d9058945a4ae47514" target='_blank'>Retracted: Efficacy of Gamma Globulin Combined with Azithromycin Sequential Therapy in the Treatment of RMPP and Its Effect on Th1/Th2 Cytokine Levels</a></td>
          <td>
            Computational and Mathematical Methods in Medicine
          </td>
          <td>2023-06-28</td>
          <td>Computational and Mathematical Methods in Medicine</td>
          <td>0</td>
          <td>2</td>
        </tr>
    
        <tr id="In the November 2017 issue, the story “Predictable Response: Finding optimal drugs and doses using artificial intelligence” (Nat. Med. 23, 1244–1247, 2017) misspelled Josep Bassaganya-Riera's last name in the second mention of his work. His last name is spelled “Bassaganya-Riera” and not “Bassanganya-Riera”.">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/f933e0ded84817f9a8edb0ca49611bdb74f3c0b2" target='_blank'>Correction</a></td>
          <td>
            
          </td>
          <td>1866-06-01</td>
          <td>Buffalo Medical and Surgical Journal</td>
          <td>0</td>
          <td>0</td>
        </tr>
    
  </tbody>
  <tfoot>
    <tr>
        <th>Abstract</th>
        <th>Title</th>
        <th>Authors</th>
        <th>Publication Date</th>
        <th>Journal/Conference</th>
        <th>Citation count</th>
        <th>Highest h-index</th>
    </tr>
  </tfoot>
  </table>
  </p>

</body>

<script>
var dataTableOptions = {
        initComplete: function () {
        this.api()
            .columns()
            .every(function () {
                let column = this;
 
                // Create select element
                let select = document.createElement('select');
                select.add(new Option(''));
                column.footer().replaceChildren(select);
 
                // Apply listener for user change in value
                select.addEventListener('change', function () {
                    column
                        .search(select.value, {exact: true})
                        .draw();
                });

                // keep the width of the select element same as the column
                select.style.width = '100%';
 
                // Add list of options
                column
                    .data()
                    .unique()
                    .sort()
                    .each(function (d, j) {
                        select.add(new Option(d));
                    });
            });
    },
    scrollX: false,
    scrollCollapse: true,
    paging: true,
    fixedColumns: true,
    columnDefs: [
        {"className": "dt-center", "targets": "_all"},
        // set width for both columns 0 and 1 as 25%
        { width: '5%', targets: 0 },
        { width: '25%', targets: 1 },
        { width: '20%', targets: 2 },
        { width: '10%', targets: 3 },
        { width: '20%', targets: 4 }

      ],
    pageLength: 10,
    layout: {
        topStart: {
            buttons: ['copy', 'csv', 'excel', 'pdf', 'print']
        }
    }
  }
  new DataTable('#table1', dataTableOptions);
  
  var table = $('#table1').DataTable();
  $('#table1 tbody').on('click', 'td:first-child', function () {
    var tr = $(this).closest('tr');
    var row = table.row( tr );

    var rowId = tr.attr('id');
    // alert(rowId);

    if (row.child.isShown()) {
      // This row is already open - close it.
      row.child.hide();
      tr.removeClass('shown');
      tr.find('td:first-child').html('<i class="material-icons">visibility_off</i>');
    } else {
      // Open row.
      // row.child('foo').show();
      var content = '<div class="child-row-content"><strong>Abstract:</strong> ' + rowId + '</div>';
      row.child(content).show();
      tr.addClass('shown');
      tr.find('td:first-child').html('<i class="material-icons">visibility</i>');
    }
  });
</script>
<style>
  .child-row-content {
    text-align: justify;
    text-justify: inter-word;
    word-wrap: break-word; /* Ensure long words are broken */
    white-space: normal; /* Ensure text wraps to the next line */
    max-width: 100%; /* Ensure content does not exceed the table width */
    padding: 10px; /* Optional: add some padding for better readability */
    /* font size */
    font-size: small;
  }
</style>
</html>