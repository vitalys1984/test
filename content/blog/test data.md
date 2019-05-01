+++
current_date = "2019-05-01T12:31:00+00:00"

+++
<ul>

{{ $data := getJSON "https://github.com/sitepoint-editors/json-examples/blob/master/src/products.json"}}

{{ range $data }}
<li>
  {{ .product_name }}
</li> {{ end }}
</ul>