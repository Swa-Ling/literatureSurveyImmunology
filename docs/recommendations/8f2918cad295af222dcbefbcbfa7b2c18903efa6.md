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
  <i class="footer">This page was last updated on 2024-09-23 06:13:13 UTC</i>
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
    
        <tr id="None">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/16a53e4f5ccd4166c9cfd1b548ed301889dc9292" target='_blank'>Seeking the ultimate challenge</a></td>
          <td>
            P. Brodin
          </td>
          <td>2019-05-24</td>
          <td>Nature Medicine</td>
          <td>0</td>
          <td>47</td>
        </tr>
    
        <tr id="Since the first introduction of Artificial Intelligence (AI) in 1956, its aim was to tackle problems with human intelligence, but with greater speed and accuracy. AI has been inspired a lot by natu...">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/51351e802ae63deeeda3a8c35429fcf87289ea58" target='_blank'>Artificial intelligence and immunotherapy</a></td>
          <td>
            Parnian Jabbari, N. Rezaei
          </td>
          <td>2019-06-03</td>
          <td>Expert Review of Clinical Immunology</td>
          <td>22</td>
          <td>90</td>
        </tr>
    
        <tr id="With the advent of effective immunotherapies to battle cancers and diseases, an obstacle in recovery has become the potential side effects, specifically cytokine release syndrome (CRS). As there is little quantitative understanding of risks for developing CRS and the degree of its severity, this work explored a model-based approach to produce a library of in silico patients through sensitivity analysis of cytokine interaction parameters and a Monte Carlo sampling. The objective of producing the in silico patients was to correlate a known grading system of cytokine release syndrome severity and thus design a new formula for grading CRS. Using our CRS grading system as the foundation, this work produced not only a formula which related the in silico patient data to the different grades, but we effectively demonstrated a selective approach to reduce the grade of CRS with sequential cytokine inhibition targets. We achieved the reduction of grades by applying the insight from the sensitivity analysis, beginning with the most sensitive targets. Cytokines IL-1, IL-8, TNF-α, INF-γ, IL-6, IL-2, IL-4, IL-10, and IL-12 were in turn the best targets for inhibition to alleviate CRS. Using this approach, patient cytokine time profiles in real-time can be related to the CRS grading system and if the grade is severe enough, action can be taken earlier during the treatment to prevent potentially life-threatening symptoms. What’s more, the identified inhibition sequence of the 9 cytokines provides guidance for clinical intervention of CRS.">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/cdbed3634ba13aed3fc2c3d954812638cfe069fa" target='_blank'>A Model-Based Investigation of Cytokine Dynamics in Immunotherapies</a></td>
          <td>
            B. Hopkins, Yiming Pan, M. Tucker, Z. Huang
          </td>
          <td>2018-12-30</td>
          <td>Processes</td>
          <td>5</td>
          <td>17</td>
        </tr>
    
        <tr id="None">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/b87d9a7e65539d9e8b8f8202e882e50d3b6daa71" target='_blank'>Amplification-Free Detection of Viruses in Minutes using Single-Particle Imaging and Machine Learning</a></td>
          <td>
            Nicolas Shiaelis, L. Peto, Andrew McMahon, Chritof Hepp, Erica Bickerton, C. Favard, D. Muriaux, M. Andersson, A. Vaughan, P. Matthews, N. Stoesser, D. Crook, A. Kapanidis, Nicole C. Robb
          </td>
          <td>2021-02-01</td>
          <td>Biophysical Journal</td>
          <td>1</td>
          <td>100</td>
        </tr>
    
        <tr id="In the last ten years, many advances have been made in the treatment and diagnosis of immune-mediated diseases [...].">
          <td id="tag"><i class="material-icons">visibility_off</i></td>
          <td><a href="https://www.semanticscholar.org/paper/6b54a56078412c3f8ce10026ceaef38f6f42908b" target='_blank'>Personalized Medicine and Machine Learning: A Roadmap for the Future</a></td>
          <td>
            M. Sebastiani, C. Vacchi, A. Manfredi, G. Cassone
          </td>
          <td>2022-07-01</td>
          <td>Journal of Clinical Medicine</td>
          <td>12</td>
          <td>42</td>
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