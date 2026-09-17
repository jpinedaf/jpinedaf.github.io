1| <h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>
2| 
3| <div class="publications">
4| <ol class="bibliography">
5| 
6| {% for link in site.data.publications.main %}
7| 
8| <li>
9| <div class="pub-row">
10|   <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
11|     {% if link.image %}
12|     <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width: auto; height: 40%">
13|     {% endif %}
14|     {% if link.conference_short %}
15|     <abbr class="badge">{{ link.conference_short }}</abbr>
16|     {% endif %}
17|   </div>
18|   <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
19|       <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
20|       {% if link.authors %}
21|       <div class="author">{{ link.authors }}</div>
22|       {% endif %}
23|       {% if link.conference %}
24|       <div class="periodical"><em>{{ link.conference }}</em>
25|       </div>
26|       {% endif %}
27|     <div class="links">
28|       {% if link.pdf %}
29|       <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">ADS</a>
30|       {% endif %}
31|       {% if link.code %}
32|       <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
33|       {% endif %}
34|       {% if link.page %}
35|       <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
36|       {% endif %}
37|       {% if link.bibtex %}
38|       <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
39|       {% endif %}
40|       {% if link.notes %}
41|       <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
42|       {% endif %}
43|       {% if link.others %}
44|       {{ link.others }}
45|       {% endif %}
46|     </div>
47|   </div>
48| </div>
49| </li>
50| 
51| <br>
52| 
53| {% endfor %}
54| 
55| </ol>
56| </div>
57| 
