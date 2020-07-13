---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true
---

# <title here>

## arks

{{ range (where .Site.RegularPages "Type" "ark") }}
* {{ .Title }}
{{ end }}