---
title: "{{ $name := substr .Name 7}}{{ replace $name "-" " " | title }}"
date: {{ .Date }}
description: 
tags:
draft: true
---
