---
layout: page
title: Products
permalink: /products/
---


<div class="home">
    <h2 align="center">Todos nuestros productos disponibles</h2>
    <div class="row">
        {% for watch in site.character %}
        <div class="col s4 m3 l4">
            <div class="card grey" >
                <div class="card-image">
                    <img src=".{{watch.image}}" style="height:200px width:150px">
                    <a class="btn-floating waves-effect waves-light red halfway-fab activator">
                    <i class="material-icons icon-plus">add</i>
                    </a>
                </div>
                <div class="card-content">
                    <span class="card-title">{{watch.title}}</span>
                    <p>{{watch.description}}</p>
                </div>
                <div class="card-action center">
                    <a href="{{watch.link}}">Oficial Site</a>
                    <a>{{watch.price}}</a>
                </div>
                <div class="card-reveal">
                    <span class="card-title">Los detalles del reloj<i class="material-icons right">close</i><p>Aqui esta todo el contenido del reloj</p>
                    </span>
                </div>
            </div>
        </div>
        {% endfor %}
    </div>
</div>

