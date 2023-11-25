---
layout: single
title: "2023/24 Round Robin Tournament"
classes: wide
---
Games to be played on the clock with a 60 minute per side fixed time period and moves recorded. Please report results to [John Schonenberger](mailto:schoneys54@gmail.com).

|Player|PA|RB|DB|BC|BD|GD|DG|CH|TH|MJ|SL|LP|DP|JS|OV|MW|AW|Score|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|Peter ALPAR|x|||||||||||||||||0|
|Raf BARGUIRDJIAN||x||||||||||||||||0|
|Doug BEER|||x|||||||||||||||0|
|Bob CLEAVE||||x||||||||||||||0|
|Bracken DAWSON|||||x|||||||||||||0|
|George DOWNIE||||||x||||||||||||0|
|David GREEN|||||||x|||||||||||0|
|Chris HUNT||||||||x||||||||||0|
|Thomas HUNT|||||||||x|||||||||0|
|Matthew JOHNSON||||||||||x||||||||0|
|Simon LAWRENCE|||||||||||x|||||||0|
|Lucasz PIECHA||||||||||||x||||||0|
|Dan PUGH|||||||||||||x|||||0|
|John SCHONENBERGER||||||||||||||x||||0|
|Oskari VIRTANEN|||||||||||||||x|||0|
|Mike WHITE||||||||||||||||x||0|
|Adam WRIGHT|||||||||||||||||x|0|
{: #results}

<style>
    /* Enable vertical table borders for this page. Tis will be overridden
    by the below script if javascript is enabled. */
    td {
        border-right: 1px solid #afa58f;
        border-left: 1px solid #afa58f;
    }

    /* Extra wide page for the table */
    .page {
        width: 100%;
    }
</style>

<script>
    let table = document.getElementById("results");
    for (var i = 1, row; row = table.rows[i]; i++) {
        for (var j = 0, cell; cell = row.cells[j]; j++) {
            // set vertical table borders to the same as bottom border
            let cellStyle = getComputedStyle(cell);
            let borderColor = cellStyle.borderBottomColor;
            let borderWidth = cellStyle.borderBottomWidth;
            let borderStyle = cellStyle.borderBottomStyle;
            let newCellStyle = "border-left:"+borderWidth+" "+borderStyle+" "+borderColor+";border-right:"+borderWidth+" "+borderStyle+" "+borderColor+";"
            cell.style = newCellStyle;

            if (cell.innerHTML == "x") {
                // Swap cells containing 'x' for solid border color
                cell.innerHTML = "";
                cell.style = newCellStyle+";background:"+borderColor+";";
            }
        }
    }
</script>
