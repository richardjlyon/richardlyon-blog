---
date: {{ .Date }}
title: "{{ $name := substr .Name 7}}{{ replace $name "-" " " | humanize }}"
description: 

type: photo
file: 
camera:     
iso:        
focallength:    
aperture:
shutterspeed:

tags:
---