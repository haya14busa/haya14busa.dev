+++
date = {{ dateFormat "2006-01-02T15:00:00Z" now.UTC }}
lastmod = {{ dateFormat "2006-01-02T15:00:00Z" now.UTC }}
author = "default"
title = "{{ replace .TranslationBaseName "-" " " | title }}"
subtitle = ""
feature = ""
tags = []
slug = '{{ .File.BaseFileName }}'
draft = true
+++

...

