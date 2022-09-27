---
toc: true
layout: post
description: Scrum Team
categories: [markdown, Week 5]
title: Javascript Fragments
author: Jishnu Singiresu
show_tags: true
comments: true
---
<script> 


let people = ["Jishnu - Backend Developer", "Luka - DevOps", "Edwin - Frontend Developer", "Emaad - Scrum Master"];


const table = document.createElement("table");
const row = document.createElement("tr");


for (let i = 0; i < people.length; i++) {
    let data = document.createElement("td");
    let node = document.createTextNode(people[i]);
    data.appendChild(node);
    row.appendChild(data);
}

table.appendChild(row);
const div = document.getElementById("JavaScriptTable");
div.appendChild(table);



</script>

<table>
    <tr>
        <td>Jishnu - Backend Developer</td>
        <td>Luka - DevOps</td>
        <td>Edwin - Frontend Developer</td>
        <td>Emaad - Scrum Master</td>
    </tr>
</table>
