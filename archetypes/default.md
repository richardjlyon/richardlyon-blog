---
title: "{{ $name := substr .Name 7}}{{ replace $name "-" " " | humanize }}"
date: {{ .Date }}
description: 
tags:
draft: true
---
