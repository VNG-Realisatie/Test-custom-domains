---
layout: page-with-side-nav
title: Documentatie StUF-EF
folder_files:
  - title: Ef0315 (zip)
    path: documenten/Ef0315.zip
    group: 315
    versie: 3.15
    status: Onbekend
    omschrijving: Behoort bij eFormulieren 1.5
    datum: 20131119
  - title: Ef0312 (zip)
    path: documenten/Ef0312.zip
    group: 312
    versie: 3.12
    status: Onbekend
    omschrijving: Behoort bij eFormulieren 1.4
    datum: 20130717
---
# Documentatie

## StUF-EF 3.15

<table>
	<thead>
		<tr>
			<th>Document</th><th>Versie</th><th>Beheerstatus</th><th>Beschrijving</th><th>Versiedatum</th>
		</tr>
	</thead>
	<tbody>
		{% for i in page.folder_files %}
			{% if i.group == 315 %} 
				<tr>
					<td>
					  <a href="{{ i.path | base_url }}">
						{{ i.title }}
					  </a>
					</td>
					<td>{{ i.versie }}</td>
					<td>{{ i.status }}</td>
					<td>{{ i.omschrijving }}</td>
					<td>{{ i.datum }}</td>
				</tr>
			{% endif %} 
		{% endfor %}
	</tbody>
</table>

## StUF-EF 3.12

<table>
	<thead>
		<tr>
			<th>Document</th><th>Versie</th><th>Beheerstatus</th><th>Beschrijving</th><th>Versiedatum</th>
		</tr>
	</thead>
	<tbody>
		{% for i in page.folder_files %}
			{% if i.group == 312 %} 
				<tr>
					<td>
					  <a href="{{ i.path | base_url }}">
						{{ i.title }}
					  </a>
					</td>
					<td>{{ i.versie }}</td>
					<td>{{ i.status }}</td>
					<td>{{ i.omschrijving }}</td>
					<td>{{ i.datum }}</td>
				</tr>
			{% endif %} 
		{% endfor %}
	</tbody>
</table>
