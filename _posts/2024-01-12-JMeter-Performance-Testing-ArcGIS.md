---
layout: post
author: Tilmann Steinmetz
---

When working with ArcGIS web services, sooner or later the question comes up: "how good will performance be, given expected usage?" Or: "how will publishing and using a certain set of services be affected by _the rest_ of the services running in the same environment?

Performance planning for Esri services can be done in more or less sophisticated ways but, realistically, performance is not known until testing the actual behaviour under a given load.

Alternatively, ArcGIS Administrators may be interested in measuring a baseline performance before publishing new capabilities. In our case I was particularly interested to get a feeling for 'normal' performance at different times of the day, considering that public users all over the world may be accessing our services with varying volumes at different times of the day. In other words, I was keen to detect whether behaviour was different during different times of the day, or on different week days. Additionally, it seemed like a great option to compare the actual performance of our Pre-Production and Production environments, respectively. The two environments are (meant to be) identical, but storage mechanisms for the attached network drives differ in practice.

The Apache JMeter tool for such testing is available free. The Esri community "Implementing ArcGIS Blog" from members of the Esri Professional Services team (https://community.esri.com/t5/implementing-arcgis-blog/recommended-strategies-for-load-testing-an-arcgis-server/ba-p/1062518) was instrumental in finally trying out the method against our ArcGIS Server services, in an ArcGIS Enterprise environment.
