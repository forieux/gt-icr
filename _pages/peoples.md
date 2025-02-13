---
permalink: /peoples/
title: "Peoples involved"
---


<div class="gallery">
{% for person in site.data.people %}
  <div class="person-card">
    <a href="{{ person.url }}" target="_blank">
      <img src="{{ person.image }}" alt="{{ person.name }}" class="person-img">
      <p class="person-name">{{ person.name }}</p>
    </a>
    <p class="person-status">{{ person.status }}</p>
    <p class="person-affiliation">{{ person.affiliation }}</p>
  </div>
{% endfor %}
</div>

<style>
  .gallery {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
  .person-card {
    width: 150px;
    text-align: center;
    border: 1px solid #ccc;
    padding: 10px;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    transition: transform 0.2s ease-in-out;
  }
  .person-card:hover {
    transform: scale(1.05);
  }
  .person-img {
    width: 100%;
    border-radius: 50%;
  }
  .person-name {
    margin-top: 10px;
    font-weight: bold;
    color: #333;
    text-decoration: none;
  }
  .person-name:hover {
    color: #007BFF;
    text-decoration: underline;
  }
  .person-status {
    font-style: italic;
    color: #555;
    margin: 5px 0;
  }
  .person-affiliation {
    font-size: 0.9em;
    color: #777;
  }
</style>


<!-- <div class="gallery"> -->
<!-- {% for person in site.data.people %} -->
<!--   <div class="person-card"> -->
<!--     <a href="{{ person.url }}" target="_blank"> -->
<!--       <img src="{{ person.image }}" alt="{{ person.name }}" class="person-img"> -->
<!--       <p class="person-name">{{ person.name }}</p> -->
<!--     </a> -->
<!--   </div> -->
<!-- {% endfor %} -->
<!-- </div> -->

<!-- <style> -->
<!--   .gallery { -->
<!--     display: flex; -->
<!--     flex-wrap: wrap; -->
<!--     gap: 20px; -->
<!--   } -->
<!--   .person-card { -->
<!--     width: 150px; -->
<!--     text-align: center; -->
<!--     border: 1px solid #ccc; -->
<!--     padding: 10px; -->
<!--     border-radius: 10px; -->
<!--     box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); -->
<!--     transition: transform 0.2s ease-in-out; -->
<!--   } -->
<!--   .person-card:hover { -->
<!--     transform: scale(1.05); -->
<!--   } -->
<!--   .person-img { -->
<!--     width: 100%; -->
<!--     border-radius: 50%; -->
<!--   } -->
<!--   .person-name { -->
<!--     margin-top: 10px; -->
<!--   } -->
<!-- </style> -->
